# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

The language is called `crontab`. [crontab.org](http://crontab.org/)


# Domain
_Describe the language's domain in five words._

Expressing when to execute commands.


# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

When someone executes a crontab program, the program parses each line from first to last. Each line 
is an expression that translates to a encoded time interval (anywhere from every few years to every minute) 
and a command. The time encoding specifies when and with what frequency the command should be executed. 
The program then runs the command each time the specified interval elapses. So, the computational model 
likely looks like a priority queue in which as each task's time comes up, it is executed and put back in 
the queue for its next time.


# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

I believe this language is very close to the "purely" domain specific side.
In this language, it is only possible to express when to do commands. The commands are written in a different language (bash). So, the
expressiveness of crontab is limited to when and what. There is no general purpose loop or conditionals built into the language, although 
there is an ability to create variables. 
It is a language that feels like a programming language with the "terseness" that Fowler seems to like. The syntax is extremely light 
weight -- a given statement has a interval 
specification and a command.


# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

This is an external DSL. It has its own syntax that is not very similar to other languages.
Although it makes use of other languages in its execution, those languages are not part of the DSL.


# Host language
_What language(s) was (were) used to implement the DSL?_

The cron utility, the main (and perhaps only) user of the crontab syntax, is implemented in `c`.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

This DSL makes it very easy to specify a task that needs to occur in a repeated manner. 
Instead of having to write a program
that has some form of daemon that runs continuously, 
waiting for a given interval to elapse 
before running a command, this DSL can be used to accomplish the same thing using a
pre-written architecture.


# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

A general-purpose language is still necessary to make use of this language. It is not
possible to specify what, exactly, to do at a given time without making use of another language. 
However, this is less of a drawback than an indicator that this is a very specific language. 
One more definitive drawback in the domain of scheduling events is that this DSL lacks an ability to specify triggers for
an event outside of time intervals. There is no
manner in which to specify that an action should occur when another event occurs.
