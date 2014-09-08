# Context Free

##  Who is this programming language for?

This programming language is for people who want to use code to make drawings
that have randomness but also allow for consistent drawing of the same image.

## What is easy to do in this language? Why is it easy?

Repeating images with shifts and decreasing size are very easy to do with 
simple recursion and scaling. Any kind of repetitive pattern is reasonably
easy to do, with only having to code out the pattern once and then define 
the shifting. It was also easy to introduce the random chances for the light
and dark green leaves. 

## What is hard to do in this language? Why is it hard?

Writing was surprisingly hard to do. Although I based my characters on the
initial “WELCOME” screen, it was harder than I expected. 
It is hard in this language to draw the exact image you want when you include
randomness. Although it is likely that one of the variants is what you want,
it takes a while to actually find it.

## How did you learn how to program in this language?

I read through some of the tutorials and looked at the “WELCOME” code. I then
tested what changing different parameters did to the picture. I repeated this
until I had a good general idea, and then came up with a picture that I liked
and executed it.

## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

ContextFree is similar to the context free grammars we learned about in 
CS81. The program starts at the startshape and expands at each step into one
of the set of commands the grammar defines for each existing symbol. Each of
these symbols then either terminates or expands into the set of commands
defined by that symbol. 

## What do you think is interesting about the ContextFree program you wrote?

As mentioned above, the characters were difficult to write, and I think they
turned out well. I introduced some randomness with the border. At each step,
the program has an option to add a larger bright green leaf or a smaller light 
green leaf. 

