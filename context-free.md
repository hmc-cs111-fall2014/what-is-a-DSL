# Context Free

##  Who is this programming language for?

I think that CF is mostly for people interested in playing with
computer art. It feels too restrictive for serious work, but for
someone who's mostly using it for fun it is very usable.

## What is easy to do in this language? Why is it easy?

It's easy to manipulate simple 2d geometric objects in simple ways
(hue changes, rotations, stretches, etc) because these are baked into
the syntax.

## What is hard to do in this language? Why is it hard?

Doing anything complicated got frustrating very quickly. For example,
I coulnd't find a straightforward way to mirror something. In general,
fine-grained control is not really what seems to be intended.

## How did you learn how to program in this language?

I followed the old 2.2 docs online, looked at the default welcome
program, and played with and poked at different ideas for a while
until I got frustrated with trying complicated things and just did
something simple. Unfortunately, the 2.2 docs were not very helpful,
but fortunately some exploring around the wiki found more interesting
things (e.g. how to use a sort of n-ary tree to randomize)

## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

In essence, CFDG nondeterministically evaluates a grammar describing
some sort of diagram, using the grammar to direct it in a Python
turtle-esque way.


## What do you think is interesting about the ContextFree program you wrote?

It randomly chooses both size and letter for each of 3 positions (the letters, of course, are HMC!)
