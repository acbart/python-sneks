In this lesson, we will learn about a new composite type named Tuples. Tuples
are similar to lists, except that they cannot be changed once they have been
created.

###  &icon-check-plus; Objectives

  1. Explain the difference between lists and tuples
  2. Construct a tuple using values, variables, and expressions
  3. Identify where tuples are commonly used in programs
  4. Write a multiple assignment statement
  5. Describe when it is appropriate to use a multiple assignment statement
  6. Define the term immutability

###  &icon-quiz; Activities

  * [#43) Lesson: Tuples](#video)
  * [#43) Quiz: Tuples](https://vt.instructure.com/courses/66476/assignments/356623)
  * [#43) Programming: Tuples](https://vt.instructure.com/courses/66476/assignments/356683)

###  &icon-educators; Lesson

Download Slides:
[Tuples.pptx](https://vt.instructure.com/courses/66476/files/5919805/download?verifier=E3i5p2dI2td6M8lZXib6PGzR7R4QBN2LfqxLQPFi&wrap=1
"Tuples.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Tuples"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/7A0aV1-q3gk?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Tuples:**  
Let's learn about Tuples

**Slide 2 - Tuples - A fixed list:**  
Tuples are a lot like lists - just a sequence of elements. However, they have
one big difference: you cannot change a tuple once its made. A list is meant
for data where you need an unknown or changing number of things. A tuple is
meant for data where you have a fixed number of things.

**Slide 3 - Tuple Literal Syntax:**  
A literal tuple value is just like a list, except instead of square brackets,
we use parentheses. Curiously, the parentheses are not technically required,
but they are almost always used.

**Slide 4 - Tuple Elements:**  
With a list, you usually want each element to be of the same type, although
technically this is not enforced by Python. Tuples, however, often end up with
many different types. In the example shown here, the tuple is composed of a
string, an integer, and a boolean . This also demonstrates how you can use
indexing syntax to access an element of a tuple.

**Slide 5 - Tuple Sizes:**  
As previously mentioned, a tuple has a fixed size. Typically, a tuple has at
least two elements, although you could conceivably create an empty tuple. The
important thing to remember is that tuples never change size once they have
been created.

**Slide 6 - Multiple Assignment:**  
So why are tuples useful? The secret is that they can show up when we want to
explicitly talk about a specific number of things. For example, you might have
a database where EVERY phone number has three parts, divided by dashes. The
following code will split the phone number into three pieces. Notice that we
have a comma separated list of variables on the left. This is known as
Multiple Assignment, and it is extremely useful and common in Python.
Remember, though, only variables and commas can be on the left side of the
equal sign.

**Slide 7 - Multiple Iteration Variables:**  
Tuples can also be used for multiple iteration variables. We actually saw this
previously when we iterated over dictionaries, and the .items() method
returned a key and value pair. This pair was actually a tuple, so we had two
variables to store each value. The built-in Zip function can actually
accomplish a similar behavior: it consumes two lists and pairs the elements
together. The name zip comes from the idea of zippering together the two
lists.

**Slide 8 - Dictionaries vs. Tuples:**  
Tuples are actually very similar to dictionaries used as records, in their own
way. Instead of using string keys, they use a numeric index. This is a trade-
off: the meaning of the tuple indexes are less clear, but they are more
concise than dictionary keys.

**Slide 9 - Tricky Commas:**  
Because the comma is what defines a tuple, a common syntax mistake is to
accidentally create a tuple. Consider the expression shown - because of the
accidental comma on the end, it will create a tuple with one string element,
instead of just a string.

**Slide 10 - Tricky Parentheses:**  
Another common mistake is to use redundant parentheses to accidentally create
tuples. This happens very easily in function calls. Notice the redundant
parentheses here pass in a tuple of four numbers to this function, instead of
passing the four numbers directly. Parentheses may seem like a harmless
addition to your code, but they can change its meaning!

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Tuples are just like lists, except they have a specific size and cannot be
changed.