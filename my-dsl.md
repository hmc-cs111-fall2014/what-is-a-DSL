# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

Alice
http://www.alice.org/index.php


# Domain
_Describe the language's domain in five words._

Object based, visual, educational PL (0)


# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

In Alice, programs are written as scripts. There are objects and methods in the world. Methods are used to directly manipulate the objects and create animations. When someone executes a program in Alice, the scripts are correlated to/translated to statements in Java. These statements are compiled and executed like Java is. This happens to produce the output, which is a smooth sequence of 3D animations. 


# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

Alice is a educational programming langauge that is full featured even though it's design domain is education (1). This means that Fowler would classify Alice like R, as a general purpose language. (2)



# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

internal
even though drag and drop
java like syntax that just covers a smaller range of expressiveness than actual java 

External. This is because although Alice is written in Java, the syntax is drag and drop blocks, which is not be a subset of normal Java syntax. 


In addition, Fowler would classify Alice as a language bench because the IDE comes with and is the only way to write Alice program. 

Source: (1)
 

# Host language
_What language(s) was (were) used to implement the DSL?_

The Java programming language. 

Source: (0)


# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

Since Alice is designed to facilitae storytelling (1), it would be easier to create stories in Alice than with a general purpose language (that is usually designed for computation). Also, it is easier to tell why a program written in Alice works because of its visual layout. 


# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

Since Alice comes with an IDE to develop in, there are a lot of preset functionality and it would be hard to say things that aren't explcitly offered as an option, i.e. it is hard to customize. 

Also, there is not very good documentation for the version 2, which might contrast to a general purpose language that is widely used by many people. (1)


# Sources

(0) http://en.wikipedia.org/wiki/Alice_(software)

(1) http://www.developer.com/java/other/article.php/3673761/Introduction-to-Alice-Programming.htm#Preface

(2) Fowler chapter 2 page 30 

