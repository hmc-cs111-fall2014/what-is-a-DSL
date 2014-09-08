# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._
SQL
[Link for the reference page of the Oracle implementation of it.](http://docs.oracle.com/cd/B19306_01/server.102/b14200/toc.htm "Oracle SQL reference")

# Domain
_Describe the language's domain in five words._
Queries and maintains relational databases

# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._
The SQL statement is parsed into instructions the database engine can understand. While parsing, it also figures out the best way to execute the query. Then, that information is passed on so that the appropriate rows in the database can be fetched or updated

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 
It is closer to "purely" domain-specific. It's designed to give instructions to relational databases.

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._
It is an external DSL. It has its own syntax and is used within programs written in other languages.

# Host language
_What language(s) was (were) used to implement the DSL?_
The original DSL was implemented in C.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_
It simplifies the process of working with a relational database, which can speed up development of a program.

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_
Though SQL is fairly straight-forward and easy to learn, it could contribute to the "language cacophany" of a program, especially if it is already using several DSLs.