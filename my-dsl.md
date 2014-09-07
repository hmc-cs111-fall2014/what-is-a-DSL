# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

[Cryptol](http://www.cryptol.net "Cryptol's Homepage")

# Domain
_Describe the language's domain in five words._

Mathematically designing cryptographic algorithms simply

# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

This language has a heavy focus on functional programming, being built 
around Haskell. Cryptol uses an interpreter to evaluate each line of a 
program. Indentation denotes blocks of code. Strong typing allows the 
interpreter to type-check before runtime. During runtime, the program 
evaluates line-by-line, interpreting the various primitive values and 
operators of the language.

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

This language is solely a domain specific language. One would not want 
to do general math in Cryptol. Cryptol would only be used to easily 
implement the functions of cryptographic algorithms. Additionally, 
Cryptol wouldn't be used to implement an entire cryptographic system, 
since the language is designed to be optimized around only mathematical 
operations. 

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

Cryptol is an internal DSL. Cryptol uses the same syntax as Haskell, 
along with many of the same keywords. As Fowler writes, since Cryptol 
only uses a small subset of features from Haskell, it feels like its own 
"custom language" instead of an external DSL like SQL.

# Host language
_What language(s) was (were) used to implement the DSL?_

Haskell

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

Implementing cryptographic functions requires correctness. One small 
mistake can break the cryptographic security. Most implement 
cryptographic functions in C, which helps to speed up functions. 
However, C is prone to errors and is far from readable. Cryptol promises 
readability, which in turn leads to code being easier to write and 
therefore being more correct.

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

Since the language is interpreted, it will never be as fast as a 
compiled language, which can use specific assembly instructions to speed 
up certain operations. Also, it isn't feasible to implement an entire 
cryptographic suite, so one will still need to rely on a general-purpose 
language.
