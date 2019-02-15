In this lesson, you will learn the difference between returning and printing
with regards to functions. You will also see the difference between printing
and calling a function.

###  &icon-check-plus; Objectives

  1. Differentiate between a return statement and a print function
  2. Identify the output of a function that does not return anything
  3. Identify the output of a function that prints instead of returns
  4. Identify a callsite

###  &icon-quiz; Activities

  * [#22) Lesson: Return and Print](#video)
  * [#22) Quiz: Return and Print](https://vt.instructure.com/courses/66476/assignments/356640)
  * [#22) Programming: Return and Print](https://vt.instructure.com/courses/66476/assignments/383584 "#22\) Programming: Return and Print" )

###  &icon-educators; Lesson

Download Slides: [Return and
Print.pptx](https://vt.instructure.com/courses/66476/files/5919802/download?verifier=ECeyG2JXxMPl9MxAXDMHLf9zA8pOtrD8bP9Wmcph&wrap=1
"Return and Print.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Return and Print"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/u20oFAgP67E?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Return and Print:**  
Let's learn about Returning and Printing.

**Slide 2 - Returning and Printing:**  
Printing and returning are two related but different ideas. However, many
beginners confuse them.

**Slide 3 - Metaphor:**  
Consider these two different scenarios. Say I ask you to recite a poem out
loud. One you are done, the poetry is no longer available to me. I heard it,
and then it was gone. This is like printing. Now, say I asked you to write
that poem down and hand it to me. The poem on paper is a concrete thing that I
could hand off to someone else, make edits to, or even destroy. This is like
returning a value.

**Slide 4 - Printing:**  
Variables and data stored inside of a computer are invisible to us. In order
to see the results of computation, we often print variables and values.
Calling the built-in print function will cause text to appear on the console.
Printing data to the console is a one-way trip, and we cannot get data written
there back.

**Slide 5 - Returning:**  
When a function is called, execution jumps to somewhere else in the program.
Some computations occur, and sometimes a result emerges. When we want to use
this result in the calling location, we need to return it. When we use the
return statement, execution jumps back to where the function was called. The
value returned is substituted in place of the function call.

**Slide 6 - Syntax:**  
Let's look at the syntactic differences between printing and returning. Return
is a special keyword statement. Print is a built-in function. This is why
print needs parentheses and return does not. Code inside of a function can
print, return, or both. But code outside of a function can print, but it
cannot return.

**Slide 7 - When to Return:**  
When someone tells you to write a function to produce a certain value, you
will need to return. The return needs to be the last thing that the function
does, because you can only return from a function once. You only ever return
inside functions, to the place where the function was called. In general, we
return data when another part of the program needs that information.

**Slide 8 - When to Print:**  
Sometimes, we write functions that print. Sometimes, we are expected to print
the result of calling a function. Sometimes, we don't print at all. You must
read instructions carefully to know what you are required to do to solve a
particular problem. In general, however, we print when we need to get
information to the user, as opposed to somewhere else in the program.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Returning from a function causes a value to be made available at the callsite.
Printing from a function makes a value appear on the console.