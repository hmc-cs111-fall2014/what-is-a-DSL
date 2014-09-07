# Context Free

##  Who is this programming language for?

The ContextFree programming language is for artists who wish to create particular pieces of art programatically. 

## What is easy to do in this language? Why is it easy?

It is easy to get started using ContextFree and create basic shapes. This is easy to do because there are several primitive shapes already included in the language, and you can see your results as you develop. I think it is particularly easy to use a language when your development and compiling environments are so closely intermingled. In Context Free, this means trying out a particular shape or design, and being able to see that image generated with the click of a mouse. This allowed me to easily experiment with several different features of Context Free and see my results (or lack thereof) right away.

Further than this, I found it very easy to work with the loops included in Context Free. It felt very natural to prototype some shape, and then work with a loop to repeat the shape many times to create the design I desired. This was easy because of it's mathematical nature: to loop 90 times, for example, one simply multiplies a statement by 90!

## What is hard to do in this language? Why is it hard?

I found it very hard to read and understand code written by other developers (on forums/in the documentation) in Context Free. Context free provides artists with a shorthand notation by which shapes can be scaled, altered, rotated, etc., and this notation is not conducive to creating readable code that can be easily understood by novices or other developers.

## How did you learn how to program in this language?

I worked through some of the examples in ContextFree's documentation and then immediately began working with some of the basics on ContextFree's IDE. While I am certainly no expert, I was able to learn the basics of using ContextFree by quickly rendering many different code segments in the development environment. 


## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

In a ContextFree program, there is a notion of a shape which is defined by some ```rule```. Any particular ```rule``` can include other rules, so one shape can be the conglomerate of several other shapes. To create an image using ContextFree, a developer simply chains together any number of rules to create some single shape, which they invoke at the top of their program using ```startshape```.


## What do you think is interesting about the ContextFree program you wrote?

I think the ContextFree program I wrote is interesting because of its relative simplicty when compared to the image it creates. In experimenting with ContextFree, I came across a way to create "spikes" by overlaying a circle in the center of a triangle. The circle covers all but the 3 points of the triangle, thus creating a spike-like image. I then learned about how to transform shapes in ContextFree, so I created a spiked trident using my original spikes shape. Taking this one step further, I was able to create an motion illusion by scaling and rotating the spiked trident about the origin. I had always wondered how one would create an optical illusion programatically, and this experience with ContextFree was my first piece of understanding how to do so.
