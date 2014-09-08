# Context Free

##  Who is this programming language for?

The ContextFree programming language is for artists to create particular pieces of art programmatically. 

## What is easy to do in this language? Why is it easy?

It is easy to get started using ContextFree and create basic shapes. This is easy to do because there are several primitive shapes already included in the language, and you can visualize your results as you develop. I think it is particularly easy to use a language when your development and compiling environments are so closely intermingled. In ContextFree, this means trying out a particular shape or design, and being able to see that image rendered with the click of a mouse. This allowed me to easily experiment with several different features of ContextFree and see my results (or lack thereof) right away.

Further than this, I found it very easy to work with the loops and control-flow mechanisms included in ContextFree. It felt very natural to prototype some shape, and then work with a loop to repeat the shape many times to create the design I desired. This was easy because of it's mathematical nature: to loop 90 times, for example, one simply multiplies a statement by 90!

## What is hard to do in this language? Why is it hard?

I found it very hard to read and understand code written by other developers (on forums/in the documentation) in ContextFree. ContextFree provides artists with a shorthand notation by which shapes can be scaled, altered, rotated, etc., and this notation is not conducive to creating readable code that can be easily understood by novices or other developers at first glance.

After using ContextFree a bit, I have been led to believe that the programming language does not lend itself to great styling standards. It seems that the more complex a particular piece of art becomes in ContextFree, the more complex the code becomes. I feel that this drawback of ContextFree is due to the very nature of the language itself, in which some rule for a shape usually depends on another shape, so the code is layered with dependencies and can be very confusing for a human to step-through and understand.  

## How did you learn how to program in this language?

I worked through some of the examples in ContextFree's documentation and then immediately began working with some of the basics in ContextFree's IDE. While I am certainly no expert, I was able to learn the basics of using ContextFree by quickly rendering many different code segments in the development environment. 


## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

In a ContextFree program, there is a notion of a shape which is defined by some ```rule```. Any particular ```rule``` can include other rules, so one shape can be the conglomerate of several other shapes. To create an image using ContextFree, a developer simply chains together any number of rules to create some single shape, which they invoke at the top of their program using ```startshape```.


## What do you think is interesting about the ContextFree program you wrote?

I think the ContextFree program I wrote is interesting because of its relative simplicity when compared to the image it creates. In experimenting with ContextFree, I came across a way to create "spikes" by overlaying a circle in the center of a triangle. The circle covers all but the 3 points of the triangle, thus creating a spike-like image. I then learned about how to transform shapes in ContextFree, so I created a spiked trident using my original spiky shape. Taking this one step further, I was able to create a motion illusion by scaling and rotating the spiked trident about the origin of the image. I had always wondered how one would create an optical illusion programmatically, and this experience with ContextFree was my first piece of understanding how to do so.
