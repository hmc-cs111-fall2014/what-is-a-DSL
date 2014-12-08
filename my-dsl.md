# Language

The language I chose is **csound**. The language, and several
IDEs for writing in it, can be found [here](http://www.csounds.com/).


# Domain
Composing and manipulating computer music.


# Computational model
"Programs" in csound are composed of two text files,
an orchestra file and a score file. The orchestra file (.orc) defines
the instruments that can be used in this performance while the score
file (.sco) defines the notes that these instruments will play. When a
csound program is executed, the computer causes the .orc file to "perform"
the score, which also contains a list of user preferences for how the
piece should be performed, generating a .wav file that can be played later.


# DSL-ness
I think csound falls fairly close to the general-purpose languages. First of
all csound is turing-complete since it has built in conditionals. This seems
like a strike against it in the "pure DSL" club. csound also allows users to
define and manipulate variables, which means that almost any problem could
be solved in csound. However, csound has no concept of dynamic input so I
would argue that it falls short of being a fully general-purpose language.
Additionally, the only kinds of output it can produce are playable audio files
so retrieving the solutions to any general problem you solve in it could be
tricky.  


# Internal or external?
csound fits Frowler's definition of an external DSL. He argues that "A
script in an internal DSL is valid code in its general purpose language",
which pretty much settles it, since csound code is nowhere close to valid
C code.


# Host language
csound was implemented in C! (c-sound). There is also some C++ and a
little bit of python in their project on [github](https://github.com/csound/csound),
but it's hard to tell what that's actually being used for. Since csound
was initially written in 1985, before python had been just as C++
was getting off the ground, it seems safe to assume that the
backend was at least initially written entirely in C.



# Benefits
This language makes it **way** easier to manage the specifics of computer
music. Trying to compose music in a general purpose language would be insane.
I would say that the main benefit of this language is the ease of composition
using its adapted syntax.


# Drawbacks
On a similar note, using this language for anything but composing music
would be insane. By using this language instead of a general-purpose one
programmer (or company) looses much of the flexibility inherent in that
language. For example being able to dynamically control the flow of code
execution goes out the window in csound. The only way to provide input
is through the static score and orchestra files. Additionally, it doesn't
seem like cscope lets you manage the specifics of the audio processing
(the number of threads it runs on, ect.), so if the user cared about
performance on a specific machine csound may not be the right choice.
