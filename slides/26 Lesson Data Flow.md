In this lesson, you will learn how data flows between functions in a program.

###  &icon-check-plus; Objectives

  1. Describe how data flows between two chained functions.
  2. Explain how values defined in one function can flow to another function.
  3. Describe how user input introduces new values

###  &icon-quiz; Activities

  * [#26) Lesson: Data Flow](#video)
  * [#26) Quiz: Data Flow](https://vt.instructure.com/courses/66476/assignments/356618)

###  &icon-educators; Lesson

Download Slides: [Data
Flow.pptx](https://vt.instructure.com/courses/66476/files/5919797/download?verifier=tamHb4MnVCNZzVQBuSNUcFN3fNF0l11t04ilKiC8&wrap=1
"Data Flow.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Data Flow"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/gtX3ZeYgeb0?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Data Flow:**  
Let's learn about Data Flow.

**Slide 2 - Scope and Values:**  
Previously, we learned about scope: the idea that variables inside a function
cannot be used outside of the function, and variables outside a function
should not be used inside the function. Further, we learned that functions do
not consume or return variables; instead they consume and return values. These
ideas are critical in understanding how data flows through a program.

**Slide 3 - Data Flow:**  
You can think of a program as a flowing, twisting river. Regular execution
makes the river flow south, but functions disrupt this flow. Along the way,
values are carried by the current. At times, we give these values names by
using variables, but it is the values that flow through the program, not the
variables.

**Slide 4 - Substitution:**  
When you call a function, each parameter is assigned the value of a relevant
argument. When you return from a function, the function call is substituted
for the returned value. These are the only tools we should use in Python to
move data around a program.

**Slide 5 - Data between Functions:**  
To move data from one function to another, you cannot just look at the two
functions. You must also look at where the functions were called. The returned
value of one function should be fed into the next function.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Data enters a function through parameters and leaves through returns. To make
data available between functions, it will need to be returned.