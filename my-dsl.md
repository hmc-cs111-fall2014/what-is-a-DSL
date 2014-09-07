# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._


[Csound](http://www.csounds.com/)

[Wiki with example code](http://en.wikipedia.org/wiki/Csound)

# Domain
_Describe the language's domain in five words._

Programming language for sound

# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

CSound allows the user to define the nature of instruments and descibe the notes and other requirements throughout time. These instructions are descibed in two different, specially formatted text files input through the command line. The instructions are processed, combined and an audio file is then the resulting output. Csound itself is written in C and is sometimes referred to as a sound compiler. 


# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

Domain specific. Doesn't seem to have many applications outside of sound manipulation, meaning it can't be used for general purposes. 


# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

CSound is an external DSL. It has its own file format (.csd) and is compiled using Csound software itself. 

# Host language
_What language(s) was (were) used to implement the DSL?_

Csound was implemented using the C language. 

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

Manipulating and handling sound within code is very difficult and most people don't know how to 
do it. With Csound, most developers are able to manupulate and test sound, and create audio files. 


# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

Can be a bit difficult to learn compared to [other programs] (https://www.flossmanuals.net/csound/) with graphical interfaces. It also requires learning how to create .csd files and a significant amount of syntax for more complicated projects. However, compared to general purpose languages it is much easier to use for manipulating sound.  