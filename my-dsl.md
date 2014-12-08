# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

[Apache Ant](http://ant.apache.org/)


# Domain
_Describe the language's domain in five words._

Describe software build processes.


# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

The Ant script is parsed down to targets with various dependencies. Ant then determines an order to execute the various tasks that satisfies these dependencies.


# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_

Ant is closer to being a pure DSL, but it is not a perfectly pure DSL. Although it's possible to write more general-purpose programs in Ant by using a target and dependency model, Ant is most often used as a simple task automation tool.


# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

Apache Ant is an external DSL because it does not use the syntax of any of its host languages. Ant buildfiles are written with XML syntax, which then needs to be parsed.


# Host language
_What language(s) was (were) used to implement the DSL?_

Ant is implemented using Java.


# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

Programmers can use an Ant script to automate the process of building large projects, which can involve many levels of depedencies and become complex and error-prone to manually keep track of.


# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

Ant script has its own set syntax that's very different from a general-purpose language. Developers have to spend the extra time reading over Ant manuals to learn this new tool.
