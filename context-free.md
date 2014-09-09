# Context Free

##  Who is this programming language for?
This programming language seems like it is mostly targeted at people who need to create graphics in a very structured way.
Those that just want to draw are paint may be better served by a tablet. However, I think there is a use case for needing a 
highly rigid, editable description for what you are creating.


## What is easy to do in this language? Why is it easy?
It is easy to adapt elements and to reuse ideas. The concept of rules makes it very easy to take one idea and use 
it a lot of times. It is also very easy to take an element and change it in a subtle way and see how the change 
affects the outcome.


## What is hard to do in this language? Why is it hard?
It is hard to build complicated computations. Multi dimensional loops are possible, but it is hard to do operations much more complicated
than addition and subtraction. I created some trees in my program, but when I looked into more complicated fractals it didn't seem
feasible. 


## How did you learn how to program in this language?
I looked at sample programs and code in the documentation, the `welcome` program, and some
forum posts that discussed tricks in the language. 


## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

A ContextFree program seems very declarative. By this I mean that it seems like programs in context free are executed as
following a tree of rules. The program begins at the root `startshape` and follows all possible rule paths until there are 
no more paths available or the paths get to small to be rendered reasonably (so recursive operations end when the recursion gets down
to the sub-pixel level).


## What do you think is interesting about the ContextFree program you wrote?
I really liked exploring the gradient abilities in ContextFree. I used a multi-dimensional 
loop to create a forest that changed hue along one axis and changed brightness along the 
second axis. I set the size such that the viewer is left with the impression that the 
forest might extend to infinity. 

