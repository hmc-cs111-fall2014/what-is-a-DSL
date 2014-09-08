# Context Free

##  Who is this programming language for?

This is for people who want to create digital art through programming.

## What is easy to do in this language? Why is it easy?

I found it pretty easy to learn the language. The syntax seemed pretty easy to understand, and because I could make small changes to my code and instantly see results, I was quickly able to figure out how things worked.

## What is hard to do in this language? Why is it hard?

When something wasn't rendering, it wasn't always easy to figure out why. The error messages provided by the GUI were not particularly helpful. The documentation also isn't the most thorough, so some things that should have been easy to figure out took more time than they should have, like changing the color of a shape.

## How did you learn how to program in this language?

I learned by looking at the official documentation. I also played around with snippets from the documentation and from the example 'WELCOME' message that showed up at startup, tweaking them slightly and seeing what the results were like. 

## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

It creates a parse tree based on your program, looking at it like a context-free grammar with circles, squares, and triangles as terminal shapes.

## What do you think is interesting about the ContextFree program you wrote?

I think one interesting thing is that when drawing a curve, it will usually draw the next segment with a square, but occasionally it will draw a circle. This is decided randomly, though squares are weighted more heavily. Every time it is rendered, there will be a random number of circles in random locations in the lines, so no two renderings from this program are alike.
