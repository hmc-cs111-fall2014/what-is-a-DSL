# Context Free

##  Who is this programming language for?

People who want to draw things

## What is easy to do in this language? Why is it easy?

Recursion is easy, since it doesn`t look like you have to explicitly specify
base cases (and it`s easy to use trial-and-error, since you never have infinite
recursion stack probelms)

## What is hard to do in this language? Why is it hard?

Loops aren`t very intuitive in this language.  It`s also hard to make shapes
that aren`t either fractals/recursive or basic builtins like circles and
triangles.

## How did you learn how to program in this language?

Trial and error.  The docs weren`t that great, so it was easier to just fiddle
with the given `Welcome` program.

## What is the underlying _computational model_ for this programming language?
_We don`t yet have a great definition of the term "computational model".
For now, try to come up with the clearest, most concise explanation of what
happens when a ContextFree program runs._

When you run the ContextFree program, it draws the shape specified by the
startshape command.  This shape may contain subshapes, which are drawn as they
are given; I would guess that the renderer basically does a depth-first
traversal of the shapes, where the leaves are builtin shapes such as circles,
triangles, and squares.  When it hits a leaf, it renders that shape and goes on
to the next shape.

## What do you think is interesting about the ContextFree program you wrote?

It`s a bug!  And kind of adorable!  It uses both recursion and loops, and also
contains nothing but circles.

There`s also a bug in the bug.  The first foot appears to have decided that it
wants to be attached the bug`s chin. :(
