# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

The language is called `crontab`. [crontab.org](http://crontab.org/)


# Domain
_Describe the language's domain in five words._

Expressing times to execute commands.


# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

When someone executes a crontab program, the program runs commands specified in the program at intervals as specified by the program.


# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

I believe this language is very close to the "purely" domain specific side of things.
In the language, it is only possible to express when to do commands. The commands are written in a different language (bash). So, the
expressiveness of crontab is limited to when and what. There is no general purpose loop or conditionals built into the language. 
It is a language though that feels like a programming language with the "terseness" that Fowler seems to like.


# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

This is an external DSL. It has its own syntax that is not similar to other languages.
Although it makes use of other languages in its execution, those languages are not part of the DSL.


# Host language
_What language(s) was (were) used to implement the DSL?_

The cron utility, the main (and perhaps only) user of the crontab syntax, is implemented in `c`.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

The DSL makes it very easy to specify a task that needs to occur in a repeated manner. Instead of having to write a program
that has some form of daemon that runs continuously, this DSL can be used to accomplish the same thing.


# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

A general-purpose language is still necessary to make use of this language. It is not
possible to specify what, exactly, to do at a given time without making use of another language.
However, even in the scope of scheduling events this DSL lacks some specificity. There is no
manner in which to specify that an action should occur when a different trigger occurs. One can only 
say to do something at a specific time and interval. 
