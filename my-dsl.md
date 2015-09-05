# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

[Lout](http://www.adrianjwells.freeuk.com/lout.pdf) is a high-level markup language, similar to LaTex.

# Domain
_Describe the language's domain in five words._

Typesetting documents, diagrams, and illustrations.

# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

Lout is a document formatter, so it reads a line of the Lout document and evaluates the expression(s) to generate a line of formatted text to add to the output document. It uses lazy evaluation to handle expressions, and can format computer program code in multiple languages, including C++, Java, Python, Perl, Ruby and Haskell.

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

If document formatting is considered to be a tight enough domain, then Lout is very domain-specific, as it was designed solely for this purpose and has practically no use outside of it.

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

This language is mostly external. It draws from Tex in some ways, but overall has its own grammar.

Here is a sample of code from the [Wikipedia page](https://en.wikipedia.org/wiki/Lout_(software)):

```
# This is a comment.

# Use the `doc' document class and its default style.
@SysInclude { doc }

@Document
@InitialFont { Times Base 10p }
//

# Beginning of document contents.
@Text @Begin

@PP
This is a paragraph.  One can easily embed @B { bold } or
@I { italic } text.  One can also easily change the style of
text, such as { Helvetica Base } @Font { changing the font
being used }.

@BeginSections
@Section @Title { The First Section }
@Begin

@PP
This is the content of a section.

@End @Section
@EndSections

@End @Text
# End of the document.
```

# Host language
_What language(s) was (were) used to implement the DSL?_

Lout was first developed with influence from the eqp equation formatter and the Scribe system, and since then the only non-original extensions and improvements were the optimal paragraph breaking and automatic hyphenation of Tex.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

Lout's biggest strangth is its ability to generate complex digrams, as well as its focus on simplicity and availability for a wide spread of users, including those who aren't familiar with programming.
It's quick and easy to learn, which companies in particular would find useful, as would programmers on a tight schedule who need to pick up a markup language and don't wish to spend time learning a more complex one.
It's also very compact taking up only 1MB of space compared to LaTex's 50-300 MB.


# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

The core language is very primitive, consisting of only a few operators. First-class functions aren't provided, and in Lout it would be impossible to, say, take in input data and generate a document by automatically adding in text and formatting.
If a company didn't need to generate complex diagrams or word and textox formatting, they may find it easier to use a simpler markup language, or one that their employees may be more familiar with, like Tex.