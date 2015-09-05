# Context Free

##  Who is this programming language for?

This is for artists who know how to program, or programmers who know how to do art. Or,perhaps, for programmers who are bored.

## What is easy to do in this language? Why is it easy?

It's easy to add simple shapes, including TITLES - words made of squares -  since these things are built in. It's also moderately easy to recursively draw a shape, as this is also a built-in function.

Plus, the 'rule's make it very easy to randomize compared to other languages.

## What is hard to do in this language? Why is it hard?

It would be difficult to generate a complex image with many strokes, such as a self-portrait, or a very complex, realistic landscape, as this language generates images that are built off of squares, circles, and triangles. It would also be difficult to do anything that isn't built in, like add a conditional statement that wasn't based on randomness or a loop that didn't run until the shapes are too small to be seen.

One very difficult thing was getting the images to stack properly. With different user-defined shapes, the order that the sub-shapes are drawn depends on their 'depth.'

## How did you learn how to program in this language?

I looked up 'contextfree tutorial', found the wiki page, went to the main page and did what it said under 'How do I get started?' This included looking at 'lesson' and 'lesson2', which are built-in 'tutorials' with well-commented code explaining how to use its functions. From there it was just trial and error.

## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

When the program runs, it renders the shapes one by one. First, the startshape is drawn, then it goes in order; if the next shape is a circle, square, or triangle, it gets drawn; otherwise, the program executes the rules, randomly choosing one when necessary. The shape the rule says to draw it added to the to do list, and this repeats until all shapes have been drawn.

## What do you think is interesting about the ContextFree program you wrote?

Pokemon is awesome! Plus, the image is composed of randomly-generated tiles, with a few overlayed squares. It's (hopefully) recognizable as MissingNo. even when randomized.