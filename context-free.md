# Context Free

##  Who is this programming language for?
This programming language seems to be for people that want to create drawings
using code. I could see it being used similarly to PostScript, where it is
usually generated programmatically by other programs. 

Alternatively, it seems like a very visual way of teaching recurrence and
loops. I could see the newer version (with more familiar syntax) as a good
teaching tool that could have been introduced, say, halfway through CS 5,
instead of turtle graphics as a way of demonstrating procedural drawing.


## What is easy to do in this language? Why is it easy?
Drawing the rainbow in my example was actually shockingly easy. Anything
involving repeated tasks with a slight change (i.e. color and size, or angle
and position) is very easy to do in Context Free. Also, randomness is very
easy, by simply making two rules with the same name, although I did not take
advantage of that fact in my example.

Those are higher level concepts, which were the first things that came to mind.
However, that is because I have just spent 4 hours in Context Free, so it seems
totally natural that I can draw a circle with ~20 characters. Looking back, the
ease with which you can draw any shape is impressive compared to the work I've
had to do to create drawings in Python or Haskell before. 


## What is hard to do in this language? Why is it hard?
Any "classical" programming task would be difficult. This is mostly because
there is no easy way to accomplish branching as far as I could tell. 

Furthermore, printing text output is incredibly difficult, as evidenced by my
"text" hello world. Normally, printing "Hello, world" is one of the easiest
things to do in a new programming language, and one of the first things I try
to learn. However, in Context Free, my rainbow took ~8 lines of code, while
"HELLO WORLD" took almost 100. I had to draw each letter manually, and while I
suppose output would be easy once ~60 characters had been defined, that is not
generally something I want to have to do going into a new programming language.


## How did you learn how to program in this language?
I learned to program in this language mostly by looking at the demo programs,
tweaking values, and seeing what happened. I looked briefly at the
documentation, but found it mostly unhelpful since we're using v2 instead of
v3. I then experimented for a few hours, and build some spirals and some
flowers. At that point, I felt like I would be able to create a rainbow fairly
quickly (and as it turned out, I could).

In general, I learned Context Free the same way I learn any language: Look at a
few examples, mess with them, and then try writing my own things with help from
documentation. I will say that context free was especially easy to learn via
messing with examples since all of the changes were instantly visible by
clicking render.


## What is the underlying _computational model_ for this programming language? 
When a context free program runs, it starts at the `startshape` and does
whatever that _rule_ says to do, following rules whenever it reaches them. If
there are multiple rules with the same name, it chooses one at random. Upon
reaching a _primitave shape_, it draws it, and then continues. Overall, it
seems like a fairly simple stack based, rule following system, similar to
purely imperative Python, except there are no assignments, and the only rules
that can be followed immediately are _paths_ or _primitive shapes_.


## What do you think is interesting about the ContextFree program you wrote?
I think the most interesting thing is the stark contrast between the small
number of lines of code required to draw a computationally intense rainbow (I'm
still impressed at how much work those 8 lines of code accomplish, and how good
it looks in the end), and the large number of lines of code required to draw a
relatively simple "HELLO WORLD". 
