# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

The domain specific language that I have chosen is Verilog. 
[Verilog's webpage](www.verilog.com)

# Domain
_Describe the language's domain in five words._

Hardware description for electronic systems.

# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

Verilog is a dataflow language in that programs consist of modules that follow 
some design hierarchy. The modules can include both sequential and concurrent 
statement blocks. Some Verilog statements can be synthesized into logically
equivalent descriptions consisting only of primitive logic statements such as 
AND, NOT, and NOR.

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

I think that from the perspective of someone who does not design computer 
hardware, it is very much so a DSL, but for someone who is focused in the domain
of computer hardware design, it would be a general purpose language. However, 
even in the case of Verilog being very DSL-ey, it is not a _pure_ DSL because
much of the language can not be used to describe hardware.

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

Verilog is an external DSL because it is a separate language with a custom
syntax designed for its purpose. It is not internal because Verilog methods 
makes sense without a larger context which is often a characteristic of internal
DSLs. 

# Host language
_What language(s) was (were) used to implement the DSL?_

I think that the host language for Verilog is the C language. It has similar
sytax and keywords and the Verilog Procedural Interface allows Verilog to 
cooperate with some C programs. 

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

One potential benefit of this lanugage is that a hardware design can be built
and simulated virtually in order to test products without having to purchase
expensive parts for designs that might not work.

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

The company would not be able to easily integrate other aspects of their work 
that are outside the domain of hardware design into the design testing, which
might limit the work that they want to do or, since verilog is not internal, 
might make the software needed to do extensive testing between hardware and 
other domains more complicated to work with.

