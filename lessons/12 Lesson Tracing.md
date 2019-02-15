In this lesson, you will learn about how variables change over time.

###  &icon-check-plus; Objectives

  1. Trace the value of a variable over the execution of a program
  2. Identify the lifetime (e.g., creation point) of a variable

###  &icon-quiz; Activities

  * [#12) Lesson: Tracing](#video)
  * [#12) Quiz: Tracing](https://vt.instructure.com/courses/66476/assignments/356645)
  * [#12) Programming: Tracing](https://vt.instructure.com/courses/66476/assignments/356659)

###  &icon-educators; Lesson

Download Slides:
[Tracing.pptx](https://vt.instructure.com/courses/66476/files/5919845/download?verifier=JDGVHISTjCRaCKZxpOuM9weAExV0URW8sM6EpJjM&wrap=1
"Tracing.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Tracing"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/0zYWaU6JJQ0?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Tracing:**  
Let's learn about Tracing.

**Slide 2 - Syntax Examples:**  
To write to a variable, you put its name on the left side of an "assignment
statement". To read from a variable, you simply use its name.

**Slide 3 - = vs. ==:**  
Notice that assignment statements use a single equal sign, and the equality
operator uses two.

**Slide 4 - Lifetime:**  
Variables have a lifetime. At some point in the program, they are initialized,
and then later on they are used. At any given time, you can ask what the value
of a variable is, and change it.

**Slide 5 - Read after Write:**  
A variable cannot be read until it has been written. If you attempt to read an
unwritten variable, an error will occur.

**Slide 6 - Update:**  
We often want to increase or decrease a variable by a variable. For instance,
when we're counting the number of things in a list, we need to add one to a
variable. We could do: x = x + 1 This really highlights the difference between
math and computing. In algebra, it would have been impossible to write that
statement, because you were solving for x. But in computing, you are ASSIGNING
to x. You are overwriting whatever was there before. That's why you should
read this statement starting from the right side. It literally means, "Take
the expression on the right and replace the variable on the left with it"

**Slide 7 - Tracing:**  
It is often useful to track the value of variables over time. We call this
"tracing" a variable. We often put these traces into a Trace Table. Although
the computer only keeps track of the latest state of the variables, we humans
want to think about the entire lifetime of the variables.

**Slide 8 - Initializing and Updating:**  
The first time a variable is written to, we say that that variable has been
"initialized" or "created". Any time after that, writing to the variable is
referred to as being "updated" or "changed".

**Slide 9 - Terminology:**  
Besides "reading" and "writing", there are many other words. You should get a
sense of the different ways we refer to variables.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

  * Automate the Boring Stuff: [Chapter 1, the second half](https://automatetheboringstuff.com/chapter1/)
  * Coding for Beginners: Pages 18-22
  * How to Think like a Computer Scientist: [2.4](http://interactivepython.org/runestone/static/thinkcspy/SimplePythonData/Variables.html)-[2.5](http://interactivepython.org/runestone/static/thinkcspy/SimplePythonData/VariableNamesandKeywords.html) and [2.10](http://interactivepython.org/runestone/static/thinkcspy/SimplePythonData/Reassignment.html)-[2.11](http://interactivepython.org/runestone/static/thinkcspy/SimplePythonData/UpdatingVariables.html)

###  &icon-flag; Summary

Variables store values so that they can be used later in the program.
Variables are created and updated using assignment statements.