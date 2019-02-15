In this lesson, you learn about the List type. Unlike the primitive types, the
List type is a complex type composed of other types. They are essential for
creating programs that do more complex and interesting things at a bigger
scale.

###  &icon-check-plus; Objectives

  1. Define the term "Composite Type"
  2. Create a list literal
  3. Identify the subtype of a list
  4. Differentiate between lists and empty lists

###  &icon-quiz; Activities

  * [#30) Lesson: Lists](#video)
  * [#30) Quiz: Lists](https://vt.instructure.com/courses/66476/assignments/356651)
  * [#30) Programming: Lists](https://vt.instructure.com/courses/66476/assignments/356672)

###  &icon-educators; Lesson

Download Slides:
[Lists.pptx](https://vt.instructure.com/courses/66476/files/5919836/download?verifier=5SyG5lkVnt1b0sqp1jt1U98bchu4aNmFezJ1R6LB&wrap=1
"Lists.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Lists"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/rgDYuhqXtjM?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Lists:**  
Let's learn about Lists.

**Slide 2 - Primitives vs. Composites:**  
We have learned about 5 primitive types: Booleans, Integers, Floats, Strings,
and the special None. Python actually has many more types, which are called
Composite types. Composite types are named because they are composed of other
types, unlike primitive types.

**Slide 3 - Lists:**  
The first composite type we will learn is the List type. A list is a sequence
of values in a specific order. For instance, you could have a list of numbers,
or a list of strings.

**Slide 4 - Lists of X:**  
A "List" is a type, much the same way that Integer is a type. However, the
List will also have a "subtype", which is what it is composed of. So if you
have a list of integers, its type is "List" and its subtype is "integer".

**Slide 5 - Defining a List:**  
We create lists using square brackets. Each value that we want to put into the
list is separated by commas. The square brackets are critical to making this a
list; without them it is not a list.

**Slide 6 - Square Brackets:**  
We've seen square brackets used before, when we were subscripting and indexing
a list. Confusingly, Python ALSO uses square brackets for creating lists. You
might struggle at first figuring out when you're looking at subscripting or
list creation. The key is whether the square brackets come AFTER an expression
- that means subscripting. If the square brackets are on their own, you have a
list.

**Slide 7 - Empty Lists:**  
A pair of square brackets with nothing between them creates an empty list. An
empty list is like an empty bag: you may not have anything in it, but you
still have the bag itself. Empty lists do not have a subtype, until you put
something in them.

**Slide 8 - Truthiness of Lists:**  
When used as a conditional, a list evaluates to True unless it is empty. This
can be very convenient when writing conditional expressions involving lists.

**Slide 9 - Printing Lists:**  
When you print a list, you will notice that the square brackets are printed
too. In fact, Python print each value of the list as if it was a literal
value. So notice that the strings have quotes around them now!

**Slide 10 - The Box Model:**  
Lists are often shown in diagrams as a row of boxes, to help us visualize the
data. Each box will have a value in it.

**Slide 11 - Terminology:**  
Some people will use the words "Array" or "Vector" to describe lists. These
are actually slightly different concepts, which we will not cover in this
course. Don't be thrown off if someone refers to a list as an "Array", but
don't use that word yourself!

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Lists are a complex type that hold multiple values at once.