# Language
_What is the name of the language? Link the name to its webpage
(if appropriate)._

[Processing 2](http://processing.org/)

# Domain
_Describe the language`s domain in five words._

Interactive design and modeling

# Computational model
_What is the underlying computational model of this language? To answer this
question, provide a high-level description (no more than 100 words) of the
computation that occurs when someone executes a program in this language._

Processing is built on Java.  It provides a scripting API for making _sketches_,
which and a lot of library functions that abstract away most of the more
nitty-gritty parts of digital modeling.

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to
`purely` domain-specific. Where does the DSL you chose fall on this spectrum,
and why?_

Processing is fairly specific -- you wouldn`t use it for anything except modeling
and animation.

# Internal or external?
_Is the language implemented as an internal or external DSL?
Justify your answer._

Processing is an internal DSL.  It is an extension of Java.

It also has a sister project, [Processing.js](http://processingjs.org/) for use
in web browsers -- this might count as an external DSL.

# Host language
_What language(s) was (were) used to implement the DSL?_

Processing was implemeneted in Java.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer`s life or a
company`s bottom line made easier by the existence of this language?_

Processing makes visual design easier, especially for artists and designers with
little programming experience.

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company
lose by using this DSL instead of a general-purpose language?_

Processing abstracts a lot away, so anything written in it might be less
optimizable than something written from scratch.
