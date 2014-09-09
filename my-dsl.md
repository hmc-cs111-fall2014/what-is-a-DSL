# Language
[Ruby on Rails](http://rubyonrails.org/)

# Domain
"Web development that doesn't hurt" That's a quote from their site. But basically web development is the domain.

# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

It's basically an add-on to the Ruby language for web development. A lot of variables and helper functions are automatically created to aid in the development of your web service based off of your naming conventions. Command line file generation creates good RESTful practice style file structures and enforce good naming conventions. Upon running everything is converted to Ruby and then to the proper html, css, and SQL commands involved. Actual HTML and CSS is also used. It does take out the need for direct SQL code. Rails would more accurately be described as a group of DSL's put together for web development.

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

It's very much DSL-like, but as I mentioned, it is more like multiple DSL's. While all the aspects of Rails specifically are very geared towards web development, its domain, there are parts for Databases and SQL and others for web page navigationa nd yet others for html generation. In that sense, it's a conglomeration of DSL's for each aspect of a much wider domain of web development.

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

It is an internal DSL, as you use ruby side by side with it and the syntax is the same as well. It is very closely coupled with its host language.


# Host language
Ruby


# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

It adds tremendously to productivity, allowing a user to get up a simple web service in minutes, with auto creation of files and semantic models for the data base. It provides auto-generated helper methods and functionality based on the file names you choose, even auto-pluralizing english words, like person to people.

It also enforces good RESTful practices. If you follow what are considered to be good RESTful design practices and naming conventions, much of the work is done for you. This stream-lines the process but also keeps the code base organized.

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

When the web service you are making is too far outside the norm, a lot of the magic of Rails must be done manuelly and is not always straight forward or well documented.

When debugging, it can be difficult when the problem is due to some of the rails magic. About half the community doesn't know how it works, just knows what functions to use, while the other half are overly adament about knowing the source code of all rails magic going on.

It is continually in development and sometimes updates are made to certain pieces you are using that are not backwards compatible. This gets bad when your project is two years old and has developed a very convoluted dependency web of something called gems. This problem mainly arises because the DSL we cal Rails is very large and perhaps has too many features. That's why it is more like a mashup of many DSL's, and perhaps it shouldn't all be one thing, but kept seperate.

That said, I love it.


