# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

[jOOQ](http://www.jooq.org/)


# Domain
_Describe the language's domain in five words._

Querying a database in Java


# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

jOOQ allows a user to easily query a database in Java using syntax similar
to SQL. When a jOOQ program is executed, the SQL-type objects are converted
into SQL queries which are then executed and the result is returned to the
program that is using jOOQ.


# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

jOOQ is closer to a “purely” domain-specific language. This is due to the fact
that it has a very limited use - just allowing users to make Java calls that
result in SQL queries. 


# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

jOOQ is an internal DSL. It is essentially an interface in Java to provide an
easy way to make SQL queries. 

# Host language
_What language(s) was (were) used to implement the DSL?_

Java was the language used to implement the DSL.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

By allowing a programmer to easily write SQL queries, jOOQ simplifies database
management and querying.


# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

jOOQ is extremely limited. A programmer or company using _only_ jOOQ would be
unable to implement much at all. If a programmer only needed the functionality
in jOOQ, they could simply use SQL. The power of jOOQ comes in making SQL-style
queries very easy in Java.
