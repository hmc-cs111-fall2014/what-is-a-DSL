# Language
[Decimal (In Python)](https://docs.python.org/2/library/decimal.html "Decimal fixed point and floating point arithmetic")


# Domain
Arbitrary precision general decimal arithmetic.


# Computational model
This language is implemented as a module within Python. When using this
library, objects of type _Decimal_ can be created. Math on these objects is
executed according to [IBM's General Decimal Arithmetic Specification](http://speleotrove.com/decimal/), 
which specifies a number of ways of performing arithmetic in a WSIWYG manner.
That is to say, inputs are taken to be whatever precision they are given as,
and are maintained in decimal notation, not in binary (the way most languages
tend to natively handle numbers, because that is the way that numbers are
implemented in ahrdware). This prevents a number of common errors associated
with floating point arithmetic, although it does come at a speed cost because
hardware does not have decimal notation built in.


# DSL-ness
This language is almost purely domain-specific. The module consists almost
entirely features that are useful for performing decimal math, and nothing
else. However, since it is implemented as a Python library, Python constructs
(such as loops, lists, map/reduce, etc.) can be used with the Decimal class to
do more complicated tasks.

Does that make it less of a domain-specific language? The module itself does
only math (and some error handling), but it can be used in a very different
way, i.e. to print numbers with a certain number of digits after the decimal
point. I guess thtis is where Fowler talks about it mostly mattering how the
language is used, as much as what the language does.


# Internal or external?
The language is implemented as an internal DSL. It is entirely implemented as a
module within Python, and it very much so uses Python's default syntax for
mathematics (by simply overloading a number of operators), and Decimal objects
can be used in other python constructs, as mentioned before.


# Host language
Python is the host language of the DSL, as Decimal is a module that can be used
in Python.


# Benefits
One benefit of the Decimal DSL is that we no longer have to worry about
floating point arithmetic issues.

For example, if we have a naive conditional check that goes as follows:
```python
a = 0.1
b = 0.3
if 9*a - 3*b == 0:
    print "Yay!"
else:
    print "What, what??"
```
Unfortunately, this will print _Wait, what??_ despite the fact that we would
like it to be the case that 9*0.1 == 3*0.3 == 0.9. However, 0.3 cannot be
represented exactly in binary, so Python struggles whith this.

Luckily, if we knew we were going to be doing a small amount of math, where we
didn't want to worry about floating point errors, we could use the Decimal
package as follows:
```python
a = Decimal('0.1')
b = Decimal('0.3')
if 9*a - 3*b == 0:
    print "Yay!"
else:
    print "What, what??"
``` 
and Python would print _Yay!_ as desired. This makes using Python for
simple personal arithmetic calculations much easier.

# Drawbacks
Unfortunately, the Decimal package has to do most of its math using software
instead of hardware. This means it is noticably slower than the default
floating point arithmetic for the purposes of large data analysis calculations.
Therefore, it is impractical to use for anything besides fulfilling a
programmer's (relatively simple) curiosity about some numeric fact.

Furthermore, while Decimal implements basic arithmetic, exponentiation and
logarithms, it does not implement some of the more complex mathematical
funcitons that a programmer might desire, such as arctan.
_
