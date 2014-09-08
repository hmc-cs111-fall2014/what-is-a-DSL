# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

Processing, [homepage](http://www.processing.org/).



# Domain
_Describe the language's domain in five words._

Image and animation rendering.




# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

The two- or three-dimensional image is rendered, I believe using an OpenGL back-end. If necessary, images are combined into animations. Existing images and data are processed as required.



# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

It's almost general purpose, in that it has a very specific domain of expertise but does not limit its expressiveness enough to be quite a DSL by Fowler's definition. 


# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

It uses Java syntax and adds a library/API/model that feels more integral to the language than a basic library. For this reason, I believe it matches part of Fowler's understanding of an internal DSL. However, it is meant to be used independently of a larger Java project, and advertises itself as its own, separate entity



# Host language
_What language(s) was (were) used to implement the DSL?_

Mostly java, some C++.



# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

Processing was initially made to have the imaging and rendering power of a more complete language like Java, but allow for more intuitive use. 



# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

It is complex enough to be used for many purposes, but the complexity is almost at the level of a general language without (readily) providing the full power and flexibility of such a language.