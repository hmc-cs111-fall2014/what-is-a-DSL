# Context Free

##  Who is this programming language for?

Context Free is for artists who want to create using programming. 
 

## What is easy to do in this language? Why is it easy?

It is easy to create pictures based in mathematical definitions in this language, i.e, recursive and fractal images. This is because you define the rules for how shapes are made and fractal/recursive rules are easy to write down in rules. Also, the program supports a pseudo form of resursion that stops when the pixel becomes to small to see (so it does terminate and you can get a static image). Also, with recursive rules, you get to define a few things and then the program does the recursive work for you. 


## What is hard to do in this language? Why is it hard?

It is hard to create discrete units and stitch them together independently in this language. This is beause sizing is relative to what is already defined and therefore it is hard to see how the current rule's sizing rules manifest on the working shape. This also makes positioning individual elements difficult.


## How did you learn how to program in this language?

I started by looking at the welcome page that popped up when you started the program and working off of that as a model for how the draw letters. That is why when I wrote a language of my name as my first program, in the extras folder. Sisi then showed me some of the recursive feature of context free and that really helped me out. I looked at the example programs as well as lesson and lesson2 to create the pretty picture. 


## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

There are two parts to ContextFree- the shapes and the rules (which apply to a shape). When a program runs, ContextFree start at the startshape rule, following it to the first defined rule. It then uses that first defined rule to modify whatever shape is currently on the working area. It repeats this (i.e. following rules) until there are no more rules, or if recursive, until the shape is too small to render (that is its stop case). If there are multiple rules, it will use the weighting factor (the number in front of the rule, default is 1 I think) to decide with what probability to pick one of those rules. 


## What do you think is interesting about the ContextFree program you wrote?

For my variant picture, I think the interesting thing about is the way the space is occupied (like where the white space is and where the picture actually occupies), due to the recursive and probalisitc nature. I included some extra work in the extras folder where I tried to sitch together indepedent elements. 
