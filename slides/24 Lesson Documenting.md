In this lesson, you will learn how to document a function.

###  &icon-check-plus; Objectives

  1. Create a single-line comment
  2. Create a multi-line comment
  3. Differentiate between a single- and multi- line comment
  4. Explain the limitation of multi-line comments
  5. Explain the purpose of documentation
  6. Document a function's inputs, outputs, and purpose

###  &icon-quiz; Activities

  * [#24) Lesson: Documenting](#video)
  * [#24) Quiz: Documenting](https://vt.instructure.com/courses/66476/assignments/356622 "#24\) Quiz: Documenting" )
  * [#24) Programming: Documenting](https://vt.instructure.com/courses/66476/assignments/383586 "#24\) Programming: Documenting" )

###  &icon-educators; Lesson

Download Slides:
[Documenting.pptx](https://vt.instructure.com/courses/66476/files/5919798/download?verifier=Mhx2J0gYmuxP2ohXm6tCiAfHxPxQ0PJDLkdydxGo&wrap=1
"Documenting.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Documenting"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/wLxhy2BB5BA?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Documenting:**  
Let's learn about Documenting.

**Slide 2 - Documenting Code:**  
Programmers write documentation in order to explain what a function does. This
is useful not only for sharing code with other programmers, but when we come
back to code we wrote later. To document code, you create comments that are
ignored when the code is executed. These comments are for the benefit of
humans, not the computer. Python has two ways of writing comments.

**Slide 3 - Single-line Comment:**  
To make a single-line comment in Python, you should use the hash symbol (also
known as "pound" or "octothorpe", written as #). Everything after the hash
symbol on the same line is completely ignored by your program.

**Slide 4 - Multi-line Comment:**  
To write multi-line comments in Python, you actually create a triple-quoted
string. When Python evaluates this string, the value is unused, so it is
safely ignored by the computer. However, unlike the single-line comment, that
means that the start of a multi-line comment must respect indentation rules as
shown here.

**Slide 5 - How Much to Comment?:**  
There are many opinions on when to write comments, and no "correct answer".
Some people believe you need to document every single line. Some people
believe you should only document functions and programs as a whole. You will
need to find your own balance - for example, rather than documenting every
line, you might only document lines that are particularly confusing, or
document a chunk of code.

**Slide 6 - Documenting functions:**  
Many people agree that, at a minimum, you should document all your functions.
Although there are many conventions, a typical function's documentation will
be a multi-line string indented as the first line of the body of the function.
This documentation should explain what 1) the function does, 2) its
parameters' types, 3) descriptions of its parameters, 4) its return type, and
5) a description of its returned value.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Documentation is a helpful tool for the benefit of programmers to better
organize code. There are several ways to document in Python, but typically
functions are documented using multi-line comments that describe the
function's inputs, outputs, and purpose.