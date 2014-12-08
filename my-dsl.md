# Language
The language is [C--](www.cminusminus.org).


# Domain
Portable quality machine code generation.


# Computational model
The computational model seems to be the same as the model used by C.  A C--
program is compiled into "quality" machine code and (presumably) run in that
form.  When a program is executed the binary code is executed on the platform
the C-- backend was targetting.

# DSL-ness
C-- is a general purpose language with a specific focus and a slightly reduced
feature set.  I would say it falls somewhere in the middle of the spectrum.  It
is still a Turing-complete, full-featured language, but it is designed for a
specific domain (producing machine code efficiently from a variety of
languages).

# Internal or external?
The language is implemented as an external DSL. It is influenced by C syntax
but does not use purely C syntax.

# Host language
As far as I can tell, C was used to implement C--, but the cminusminus site is
really sketchy on those kinds of details.

# Benefits
C-- provides support for optimized tail calls, exceptions, and lightweight
concurrency.

# Drawbacks
C-- does not provide varargs procedures, unlike C.
