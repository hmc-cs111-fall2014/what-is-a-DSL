# Context Free

##  Who is this programming language for?
People who want to draw interesting images without having to know the details of
image generation/drawing/grapics/etc, or people who want to try to draw
interesting things without even necessarily knowing what they're doing.

## What is easy to do in this language? Why is it easy?
Drawing any kind of interesting picture is easy.  Any valid code will produce a
picture, and it's really simple to make the image somewhat interesting by adding
rotation or messing with hues.  Depending on how simple of an example you
choose, it's even possible to take existing code and modify it to get something
else interesting.

## What is hard to do in this language? Why is it hard?
It's hard to define clean and nice to use subroutines in this language.  The
rules are confusing and I don't think I quite understand how they work (besides
being expanded by the language somehow).  Looping seems really limited.
Rotating is easy, because you can apply the rotate operation multiple times, but
it's hard to do, say, a color gradient, because you can't apply a hue operation
multiple times.  It'd be nice if I could change some variable or increment
something with a proper loop operation.

## How did you learn how to program in this language?
Basically by a combination of reverse-engineering other examples and messing
around with numbers until I liked the resulting picture. Trial-and-error,
basically.  I tried to reverse-engineer the tree example, failed, messed around
with squares, noticed I could get a spiral-y thing with rotated squares, and
messed around with that more until I liked the result enough to stop.

## What is the underlying _computational model_ for this programming language? 
As far as I can tell, ContextFree expands rules out by pasting in other rules
until you just have a list of operations or shapes to be drawn.  It then goes
through all of these operations and applies them to draw the final shape.  I
gathered this from when I accidentally made ContextFree loop forever (or at
least for a long time) and it mentioned having to expand a lot of rules to get a
lot of shapes.

## What do you think is interesting about the ContextFree program you wrote?
It's really simple, but still produces an interesting pattern.  The crossed
lines look really cool and I like how they meet to form a spiral in the middle.
I especially like the white band that seems to be present near the outside of
the image - that was entirely accidental.
