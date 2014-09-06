# Context Free

##  Who is this programming language for?

This programming language is for artists and programmer who want to make patterned digital graphics.


## What is easy to do in this language? Why is it easy?

It's easy to draw patterns made of repeated simple shapes, such as fractals. Context Free have easy syntax for modularization and a simple model for manipulating a defined shape through various transformation.


## What is hard to do in this language? Why is it hard?

Drawing a complex shape that cannot be broken down into repeatable pieces is difficult. Shapes such as a stick figure or a word require many components that cannot be easily reused, so the programmer has to configure each one separately.


## How did you learn how to program in this language?

I learned by looking at simple examples and manipulating different parameters to observe what the changes in code did to the rendered picture.


## What is the underlying _computational model_ for this programming language? 

_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

When a ContextFree program runs, rules are executed in sequential order. The program adds basic modified shapes one at a time, until termination conditions are met.


## What do you think is interesting about the ContextFree program you wrote?

My program is interesting in that the only shape it uses is circles, but by leveraging several powerful tools in Context Free, I made an interesting and relatively complex image. I used infinite recursion to produce the pattern, making small modifications at each step to make it interesting. The program also contains random components, so it can generate many slightly different variations of the pattern.

