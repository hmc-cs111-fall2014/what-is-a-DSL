# Context Free

##  Who is this programming language for?

Context Free appears to be for artists (or hobbyists interested in creating
art). However, given that Context Free is a programming language, a more
suitable audience is the subset of artists who can program.


## What is easy to do in this language? Why is it easy?

Repetition and recursion are extraordinarily easy in Context Free because
the rule-based syntax supports recursive rule definitions. (Interestingly,
it seems that a base case is not necessary when writing recursive rule
definitions). Furthermore, Context Free makes randomness extraordinarily
easy, as it will just pick randomly between rule definitions with the same
name (respecting to the user-provided weights). 


## What is hard to do in this language? Why is it hard?

Context Free excels in performing any sort of repetition or recursion, but
the language would be much harder to use for more difficult and complicated
artwork without repetition. The reason for this is that each basic shape or
stroke must be defined in the program. Without the aid of recursion, manually
defining many shapes would be a rather tedious and frustrating task. Though
my artistic expertise is limited, this seems to suggest that Context Free is
generally more challenging to use for non-abstract art.


## How did you learn how to program in this language?

I started to learn how to program in Context Free by looking at the provided
example programs. Then, once I had a basic idea of the structure of the code,
I skimmed the Context Free documentation to get a better understanding of the
language. I also had to do some deep searching in the documentation and some
experimentation with the examples in order to figure out how randomness was
introduced to Context Free programs (as it wasn't intuitively obvious to me
initially).


## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

A Context Free program appears to be similar to a context-free grammar (which
seems to explain the name). A program is a series of rules, and each rule
defines one or more basic shapes (terminal elements of the grammar) or other
rules to be drawn. Recursive rules allow for just a few rules to generate
many shapes, and Context Free chooses between rules of the same name randomly
(respecting user-specified weights). A base case does not need to be specified
for recursive rules, which suggests that Context Free will recurse until
additional recursion ceases to change the end result. This entire drawing
process is triggered by the `startshape` command.


## What do you think is interesting about the ContextFree program you wrote?

I think that the Context Free program I wrote is interesting because it
incorporates many key features of Context Free: repetition, recursion, color,
and random rule selection. Furthermore, he changing colors of the overlapping
swirls help illustrate the order in which the swirls were drawn (as the
lighter-colored parts are on top of the darker-colored parts). Finally, though
it's certainly subjective, I think that the end result looks reasonably cool.
