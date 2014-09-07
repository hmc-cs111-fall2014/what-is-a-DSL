# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

[Fabric](http://www.fabfile.org/)


# Domain
_Describe the language's domain in five words._

SSH deployment and remote execution


# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

At its core, Fabric is a Python library and a command line tool. A fabfile is
a Python module that contains functions describing actions to be performed on
remote machines, and running the fab tool runs the commands in the fabfile
on remote machines. Beyond the list of commands to be run remotely, the fabfile
can specify details such as whether remote machines should be accessed sequentially
or in parallel, and this additional information influences how the fab tool performs
the remote execution.

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

Because Fabric is an internal DSL (as described below), it doesn't really have enforce
concept of limited expressiveness. That said, though, Fabric (as opposed to its host
language, Python) only provides a small handfull of functions, decorators, and
context managers which all explicitly relate to the configuration and execution of
remote command execution via SSH. In that sense, then, Fabric is closer to the "purely"
domain-specific end of Fowler's spectrum. In any case, Fabric commands are typically used
in indepdendent "fabfiles," isolated from other Python code and run only via the fab tool,
which makes Fabric scripts appear visibly distinct from standard Python programs.


# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

Fabric is an internal DSL. It is really just a Python library that is used as a DSL,
so every line of code in a Fabric script is a valid line of Python code. Furthermore,
Fabric commands can be easily interspersed throughout Python programs, though it isn't
this usage of Fabric as a library that I consider when thinking of Fabric as a DSL.


# Host language
_What language(s) was (were) used to implement the DSL?_

Fabric is implemented entirely in Python.


# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

Fabric abstracts away a lot of the overhead that comes with deployment, particularly
deployment to multiple machines. It allows developers to focus on the commands that they
would like to run on remotely instead of on the logistical details of how to connect to
those machines.


# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of general-purpose language?_

Because Fabric is an internal DSL, using Fabric does not prevent the use of general-purpose
Python. However, because Fabric abstracts away much of the overhead associated with remote
code execution, it is not always clear how exactly a fabfile gets executed on remote machines.
Thus, for more complicated use cases, a basic understanding of Fabric's underlying execution
model and concepts such as pseudo-tty may be necessary. This can take some time to learn
(and can also ruin some of the "magic" of Fabric).
