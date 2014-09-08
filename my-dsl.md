# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

   The name of the language is [Csound](http://www.csounds.com/).

# Domain
_Describe the language's domain in five words._

   Modular and extensible audio programming.

# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

   Wave files are produced using _orchestra_ and _score_ files that define the instruments, notes, and other audio parameters. This is done through unit generators (also known as opcodes), which use predefined arrays of values that describe waveforms of specific frequencies. If the waveform is not predefined, the unit generator uses the function for that waveform to determined the values.


# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

Csound is at a point in the spectrum close to a "purely" domain-specific language, as all it is really used for is for audio programming or as a sound compiler. Csound is easily extensible as it is completely modular, the expressiveness of Csound is limited in that it can only be used to define different sounds at specific points in time.

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

Csound is an external DSL, because although it is written in C it is self-contained and separate from C. Csound uses syntax that would not be valid in C, and thus cannot be an internal DSL.

# Host language
_What language(s) was (were) used to implement the DSL?_

C!

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

This language offers a lot of flexibility over synthesized audio as you can very carefully articulate exactly what type of instruments, notes, and timing you want. Also, because there are already many unit generators, Csound can make synthesized sound very cheap as you do not have the cost of instrumental recordings and such if you were to do it in a general-programming language (although libraries could exist for that in some languages as well)


# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of general-purpose language?_

Hand coding the _orchestra_ and _score_ files can become tedious, which combined with the limits of the strict syntax, can make it pretty difficult to truly express the music the programmer/composer is trying to create. The one way to overcome this drawback is to use Csound in conjunction with another language/tool, which still has the downside of making it harder to connect all of the pieces and logic.