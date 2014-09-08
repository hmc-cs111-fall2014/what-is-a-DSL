# Context Free

##  Who is this programming language for?

I could see Context Free being used as a language for artists
(with at least some programming background), almost like a unique 
medium.

## What is easy to do in this language? Why is it easy?

The nature of functions and simple recursion make this language great
for images with repeated patterns. I also really like how loops can
be written with a transformation to occur each step of the loop, 
it allows for nice gradients and size changes, etc.

## What is hard to do in this language? Why is it hard?

Making realistic/less abstract art seems incredibly difficult, because
any shape you want to draw needs to be composed of circles squares and
triangles, so you really need to build from the ground up.

## How did you learn how to program in this language?

I started by looking at the pre-installed example programs. From there I took
snipets and messed around manipulating them, and tried to do some things of
my own (such as make a fake mandlebrot fractal that would look vaguely like
the real one). As I continued working, I gained more proficiency with the
aspects of the language I was using, though not with a whole lot else.

## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

Rules are followed with some stack of transformations to be applied until a
base shape is hit. That shape is drawn with those transformations, then
traversal continues, moving back up the stack when appropriate and down into
new leaves, etc, until all rules have been executed/some minimum size of a
shape is hit (at which point that branch will move back up the stack), or
the image overflows.

## What do you think is interesting about the ContextFree program you wrote?

I did two interesting things with my program: I tried to make it from 
scratch, and I tried to create a non-abstract picture. For the former,
I mean that after looking at examples, I then closed their code and opened
a blank document, so that the image would accurately reflect my understanding
and abilities with context free. For the second, I actually started making
abstract shapes, but then decided that was boring and wanted to see just
how difficult making more typical images might be.
