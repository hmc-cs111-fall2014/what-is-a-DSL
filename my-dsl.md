# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._
[Robot Battle Scripting Language (RSL)](http://www.robotbattle.com/gamedocs/)

# Domain
_Describe the language's domain in five words._
Video game with battling robots.

# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._
As best I can tell from the game's 
[source code](http://dev.robotbattle.com/cgi-bin/viewvc.cgi/rbdev/win32/trunk/),
RSL files for the various robots are simplified (such as by evaluating
addition/logic/trig functions) and stored in "Code" objects which are a
series of characters representing different actions. Thus, the "Code"
object is a machine code-esqe string of tokens. This is then
interpreted by a translator as events occur and the robots make moves in a
battle. So in some sense, the game code is acting as a VM, which compiles and
then runs the robot code according to the game rules.

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 
RSL is _almost_ purely domain-specific. While one could in theory set up
multiple robots and configure an arena (I think that's possible, though through
the game not RSL) specifically to perform some sort of calculation, this
language really is not intended for anything beyond controlling your
robot in the game, and doing so would be difficult (while some structures
like functions, conditionals and loops are provided, these are primarily
event-driven, and I don't think you can define any variables).

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._
This DSL is external. It has its own special allowable syntax and commands,
and these are parsed and translated for use by the host language.

# Host language
_What language(s) was (were) used to implement the DSL?_
RSL is hosted on C++ (see the game's source code link above)

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_
RSL allows players to create their robot AI for the Robot Battle video
game without needing to know about the underlying implementation of the game
or how to code in any other languages. It is designed to be reasonably simple
and scoped for a beginner to get a robot moving and shooting, but complex
enough that a strong programmer can develop a complex AI.

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_
One downside of this language is that any complex AI algorithms developed
are not immediately portable to a more general purpose; it would take a
non-negligible amount of work to translate and abstract them to another context.
