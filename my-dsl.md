# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

The domain specific language I have chosen is [Apache Ant](http://ant.apache.org/).

# Domain
_Describe the language's domain in five words._

Build process for Java applications.

# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

Ant is used to explicitly establish a build process and dependencies for Java applications. Build processes written in Ant specify named targets and their associated dependencies. Targets are composed of actions to be performed on specified paths, such as ```javac```, ```jar```, ```mkdir```, and ```delete``` (among others). Ant then establishes dependencies between different build targets and performs the specified actions in the order that satisfies these dependencies. This allows developers to easily control every step of the Java build process, from the initial directory setup, to the invocation of the Java compilier, to the creation of a Java executable (```jar```) file.


# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 


# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._


# Host language
_What language(s) was (were) used to implement the DSL?_


# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_


# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_
