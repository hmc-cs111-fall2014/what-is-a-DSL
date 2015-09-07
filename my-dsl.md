# Language
[Protocol Buffers](https://developers.google.com/protocol-buffers/)


# Domain
Sending and processing language-neutral data.


# Computational model
The file that defines the messages is compiled, and then instances of the messages used by other applications are encoded to binary based on the object file.


# DSL-ness
Protocol Buffers falls much closer to the domain-specific side of the spectrum. Fowler often refers to whether a language supports conditional logic and looping to determine whether it's general-purpose, and as far as I know, Protocol Buffers supports neither feature.


# Internal or external?
Protocol Buffers is an external DSL as it does not employ the syntax of the language in which it's written.


# Host language
There's an implementation of Protocol Buffers for each language the DSL supports: Java, C++, Python, JavaNano, Ruby (and I think others).


# Benefits
Protocol Buffers allows users to transfer data across applications--potentially, even if the applications are written in separate languages. The DSL also generates classes for the defined messages to more easily set and access the message fields.


# Drawbacks
With respect to XML, Protocol Buffers is not designed to model structure and is not as human-readable.
