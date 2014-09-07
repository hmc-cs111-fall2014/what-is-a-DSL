# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

The domain specific language I have chosen is [Apache Ant](http://ant.apache.org/).

# Domain
_Describe the language's domain in five words._

Build process for Java applications.

# Computational model
_What is the underlying computational model of this language? To answer this 
question, provide a high-level description (no more than 100 words) of the 
computation that occurs when someone executes a program in this language._

Ant is used to explicitly establish a build process and dependencies for Java applications. Build processes written in Ant specify named targets and their associated dependencies. Targets are composed of actions to be performed on specified paths, such as ```javac```, ```jar```, ```mkdir```, and ```delete``` (among others). Ant then establishes dependencies between different build targets and performs the specified actions in the order that satisfies these dependencies. This allows developers to easily control every step of the Java build process, from the initial directory setup, to the invocation of the Java compilier, to the creation of a Java executable (```jar```) file.


# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

While Ant certainly has a clear and specific domain focus, Apache's documentation on Ant details the [extensive array of tasks](http://ant.apache.org/manual/tasklist.html) which can be performed using Ant. Furthemore, developers can [implement their own tasks](http://ant.apache.org/manual/develop.html) for build processes (or even other functions). This seemingly unlimited range of expressiveness characterizes Ant as more of a general-purpose language than a purely domain=specific language.

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

Ant is implemented as an external DSL. To use Ant, a developer creates a ```build.xml`` file ([by default](http://ant.apache.org/manual/running.html#commandline)), which specifies a series of targets, actions, and dependencies using XML. Thus, in the context of a Java application, Ant invokes its own syntax and style, and is therefore classified as an external DSL. 

# Host language
_What language(s) was (were) used to implement the DSL?_

Ant is hosted in the Java programming language, and is most commonly found as a component of the build process of a Java application. An Ant file is written by a developer in XML, which is then parsed and executed in Java.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

Apache Ant allows developers to explicitly specify the build process and associated dependencies for a Java application. This provides developers with a modular and scalable solution to creating the build process for their applications. For any company, this means spending less time debugging the build/deploy process, less time integrating new team members, and less time integrating new dependencies into an existing application.

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

Because Ant relies so heavily on the use of XML, a simple Java application might have an unncessarily complex and verbose XML build specification. This highlights one of the main drawbacks of Ant: build processes may seem unwiedly and excessively long when sepcified in XML. To combat this drawback, though, [several IDEs](https://ant.apache.org/manual/ide.html) now natively integrate Ant to allow developers to more easily visualize and manage their Ant build proccesses.
