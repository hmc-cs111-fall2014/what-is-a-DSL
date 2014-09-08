# Context Free

##  Who is this programming language for?

Anyone who wishes to design artwork using code.

## What is easy to do in this language? Why is it easy?

Designing digital art can be very difficult. It's easy to create basic 
shapes in this language.

## What is hard to do in this language? Why is it hard?

Individual shapes or rules do not have identifiers, so I could not 
easily place additional shapes in alignment with other shapes. Each 
shape had to be tweaked in regard to its x and y placement.

## How did you learn how to program in this language?

I learned through examples. I went through many of the pieces of artwork 
in the gallery and learned syntax and features from them. I also read 
through some of the basic documentation.

## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

The language is interpreted. It begins with the method 'startshape 
RULE,' where 'RULE' is some rule one wrote. When the program hits a rule 
it doesn't know, it looks for a rule that a user defined. If it exists, 
it jumps to that rule and executes it before jumping back to the 
previous rule. This continues until the program runs out of 
instructions. If the program gets into a loop due to recursion, it will 
exit if the images it is drawing become too small.

## What do you think is interesting about the ContextFree program you wrote?

The program is based off the Pythagorean theorem. I also love to doodle 
whenever I have paper in front of me, and I typically create spirals. 
Combining both of these, I designed a visual representation of the 
Pythagorean theorem that spiraled inwards.
