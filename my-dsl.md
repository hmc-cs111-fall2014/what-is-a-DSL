# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._
The name of the language is django.
[Django Project](https://www.djangoproject.com/)

# Domain
_Describe the language's domain in five words._
Open-source rapid web application development

# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._
When someone executes a program using Django, it is interpreted as a Python program. When certain requests are made, the request is converted to a series of SQL statements that alter a database to follow a data model.

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 
Django is leaning towards a domain-specific language because it is specific to rapid web application development. Django is written and used for database control as it relates to web applcations.

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._
Django is an internal DSL because Django is a set of Python libraries. 

# Host language
_What language(s) was (were) used to implement the DSL?_
Django is written in Python.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_
By building a web application using Django, developers can take advantage of a Model-View-Controller pattern. Django allows developers to change one part, such as the view, of a web application without the need to alter another part, such as the model.

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_
By using this DSL, the program has the overhead of the Django framework. A programmer also loses granular control of the underlying model and has to deal with maintaining code to keep up with changes to the framework.