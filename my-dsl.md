# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

SBT: http://www.scala-sbt.org/0.13/docs/index.html

# Domain
_Describe the language's domain in five words._

Defining build process for Scala

# Computational model
_What is the underlying computational model of this language? To
answer this question, provide a high-level description (no more than
100 words) of the computation that occurs when someone executes a
program in this language._

SBT is actually a combination of a language
and a program. It provides a shell with various extended functions
such as automatically finding and running tests with a single, 0
argument command. The language itself provides a simple mechanism for
specifying dependencies, sources of those dependencies (e.g. a github
repository, versions of the deps, version of the program itself, and
so on.

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

I believe SBT falls well on the "DSL" side of the spectrum. It is
obviously a computer language of some sort (it does actually encode
instructions to a machine). It isn't a set of library calls; it has
various operators (e.g. %, %%, :=). It has limited expressiveness: its
operators are targeted at specifying things in its domain, and they
make working outside that domain very difficult.

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

I consider SBT to be an external language. While it is possible to
define its operators in Scala (that is the host language, after all),
without explicitly making those definitions it is not valid Scala
code.

# Host language
_What language(s) was (were) used to implement the DSL?_

SBT is written in Scala.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

SBT provides a unified environment for building, testing, and running
a code base. It does the heavy lifting for handling deep dependencies,
strange dependency graphs, etc. It provides a simple way to specify
the version and source of a dependency, if desired.

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

SBT (in my view) adds unneeded extra work to understand a program's
build configuration. The operators' meanings are sometimes
non-obvious, and much of the configuration could easily be handled in
a more typical configuration file.
