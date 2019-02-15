This lesson shows how lists are different from other types because they are
mutable (the variable's value can be changed, as opposed to taking on a new
value).

###  &icon-check-plus; Objectives

  1. Define the term Mutability
  2. Differentiate list appending from string addition
  3. Explain the result of assigning the result of list appending to the list variable

###  &icon-quiz; Activities

  * [#34) Lesson: Mutability](#video)
  * [#34) Quiz: Mutability](https://vt.instructure.com/courses/66476/assignments/356600)
  * [#34) Programming: Mutability](https://vt.instructure.com/courses/66476/assignments/393637 "#34\) Programming: Mutability" )

###  &icon-educators; Lesson

Download Slides:
[Mutability.pptx](https://vt.instructure.com/courses/66476/files/5919801/download?verifier=jg0Cfguc6McVZ2NsuQNxo7OE2exYA4cYihDKpdUM&wrap=1
"Mutability.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Mutability"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/dh0vLw2Pmjk?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Mutability:**  
Let's learn about Mutability.

**Slide 2 - Mutability:**  
Strings and lists are similar because they are both sequences of elements.
However, a big difference between them is their Mutability. Strings are
immutable while lists are mutable.

**Slide 3 - Immutable Strings:**  
Say you have a string variable. When you add another string to that variable,
you need to assign the result - otherwise it is lost. Similarly, when you call
a string method, you need to assign the result - otherwise it is lost. This is
the idea of immutability - you are never changing the string, you are simply
creating new ones.

**Slide 4 - Mutable Lists:**  
Now say you have a list variable. When you append a value to that variable,
you must not assign the result back. The append method modifies the list
variable, and then returns None, so if you assign its result you overwrite the
list variable. The append call mutated the list - it changed the data inside
the list without affecting the list variable.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Lists can have their value changed, unlike other types of values like strings.