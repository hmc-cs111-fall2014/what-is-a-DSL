# Context Free

##  Who is this programming language for?

Those that want to create art with programs, with a focus recursion. It is possible it is usable by someone who is just learning about programming.

## What is easy to do in this language? Why is it easy?

It is easy to draw cool, repetitive patterns. Recursive drawing has built in base case that allows you to play with the pattern and not worry about the program running forever. It stops the recursion once it becomes to small to see. It also has some built in randomness, to make more organic looking patters like trees.

## What is hard to do in this language? Why is it hard?

To make non-basic shapes that would normally be easily defined by a function or formula. There are no conditionals or variable to speak of, so creating a sine wave would be very difficult.

## How did you learn how to program in this language?

I looked through and played with the various examples it came with.

## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

There a few basic shapes that are objects with a heading and a relative size to other shapes. Through recursion, with some automatically generated base cases of proportional size, all the basic objects are created and rendered following the users' instructions or rules.


## What do you think is interesting about the ContextFree program you wrote?

I took advantage of the automatic randomness feature. It's a bit of a throw back to random walks from CS5. By weighting stopping of movement very low, I could randomly generate very long, convoluted paths. I think this program reveals the order of rendering a bit too, as you can see the overlap of the path onto itself.
