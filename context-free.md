# Context Free

##  Who is this programming language for?

This language seems best suited to people who want to make somewhat intricate art.
I imagine that it is mostly used by semi-technical enthusiasts, but could be used by others too.

## What is easy to do in this language? Why is it easy?

I found recursive or fractal structures to be exceptionally easy to make because of the natural way in which rules
can reference themselves.

I also found transformations of scale, color, and position to be very easy to do thanks to the 'shape adjustment' system.

## What is hard to do in this language? Why is it hard?

I found that this language makes it hard to tackle a particular shape. For example, when making the Koch Snowflake I
ended up with a whole bunch of interior triangles, mostly because I didn't have any good ways to get rid of the without
messing up the recursive structure.

Put more formally, because this language allows you to creat so many shapes, it then becomes challenging to single out particular ones to modify.

Perhaps this could be achieved by having a way of selecting an already drawn shape to modify/delete? Although that would mess up the whole draw-only philosophy of the language, and could potentially cause other problems.

## How did you learn how to program in this language?

I started working with the language by modifying the examples and seeing what happened.
I then moved on to trying to build my own art.
I frequently got stuck on something and would either
  - Work through it (painful, but also valuable)
  - Look at the documentation

## What is the underlying _computational model_ for this programming language? 

When a ContextFree program runs:
  1. The code is parsed by the application.
  2. The application starts with the starter rule and draws it to the output image.
  3. The program may draw _many_ nested shapes (and primitive shapes) as a part of this process.
  4. It may also apply many transformations along the way.
  5. If rules get to a very small scale, it doesn't draw them.

For what its worth I believe the application is implemented in C/C++ from the source/build system.

## What do you think is interesting about the ContextFree program you wrote?

I liked making a program that took advantage of recursion, which was very natural in the language.

Additionally, while my program took a disproportionately long time to write, I sort of enjoyed the derpy process
and all that I learned along the way.
