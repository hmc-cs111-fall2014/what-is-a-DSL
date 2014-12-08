# Context Free

##  Who is this programming language for?
This programming language appears to be for mathematicians/computer scientists who
have some mathematical object that they wish to be able to visualize. It does
not seem to be intended for artists or someone picturing an image and wanting to
display that image on a computer screen, since it is extremely difficult to figure
out how to draw most things.


## What is easy to do in this language? Why is it easy?
It is very easy to produce patterned shapes, i.e. those created by recursion or
looping. This is easy because recursion is one of the basic architecture types
for creating a rule, and it is extremely easy to build in rotations and
other transforms that produce regular images. In this vein, fractals are a very
simple output of this language. Additionally, basic shapes and mathematical transforms
of basic shapes are easy, since the primitives of the language include basic shapes.


## What is hard to do in this language? Why is it hard?
As previously mentioned, it is difficult to represent images in the way an artist
might expect. This is hard because the computer requires some mathematical description
or recursive definition for curves and patterns, making arbitrary curves and lines
extremely difficult. Of course, most things outside the context of drawing and geometry
are also very difficult or impossible in this language, since it doesn't have the
general-purpose tools for essentially any task other than drawing.


## How did you learn how to program in this language?
I read some of the online documentation in order to become familiar with the syntax of
the language. Then, I took an example and tinkered heavily in order to actually understand
what different modifications would do. For this purpose, I commented out most modifications
and slowly built up an understanding of what each part of the example did and how it
affected the output of the program. Finally, I tried to create my own example with similar
shape modifications.


## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._
The entire program runs on top of a planar world view in which there is a single pen that
has knowledge of x and y coordinates as wells as derived concepts such as angle and width.
When a program runs, rules are executed in depth-first fashion, starting with the declared shape
to be rendered. Recursive rules are executed until no longer visible. The world view is maintained
at each level of state so that the ending point of the pen after one rule call does not dictate
the starting point for the next rule.

## What do you think is interesting about the ContextFree program you wrote?
I think there are several factors of note in the program. One is the choice of size and rotation
angle for each helix. They are chosen visually so that the loops of each spiral just barely
touch when done with triangles. Similarly, the rotation of the three helixes mean that the
three central triangles are aligned. I also enjoy the patterns created by the overlapping of squares,
triangles, and circles. Finally, I think the stacking of rules (drawHelix having calls to each type
of helix, and then drawHelixes having multiple calls to drawHelix) highlights the concept of
how rules exist as a data type for the language, and demonstrates the structure of ContextFree.

