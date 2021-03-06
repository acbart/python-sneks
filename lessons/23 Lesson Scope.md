In this lesson, you will learn how the "scope" (or availability) of a variable
changes with respect to a function.

###  &icon-check-plus; Objectives

  1. Determine whether a variable is available within a function.
  2. Determine whether a variable is available outside a function.
  3. Determine whether a variable is aliased within a function.
  4. Define the difference between a global variable and a local variable.
  5. Explain why global variables are bad.

###  &icon-quiz; Activities

  * [#23) Lesson: Scope](#video)
  * [#23) Quiz: Scope](https://vt.instructure.com/courses/66476/assignments/356625 "#23\) Quiz: Scope" )
  * [#23) Programming: Scope](https://vt.instructure.com/courses/66476/assignments/383585 "#23\) Programming: Scope" )

###  &icon-educators; Lesson

Download Slides:
[Scope.pptx](https://vt.instructure.com/courses/66476/files/5919803/download?verifier=JGTVMTricfvrj25x7QmbSyKNcpiixgAn52BLJHTt&wrap=1
"Scope.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Scope"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/uaMbB17yg64?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Scope:**  
Let's learn about Scope.

**Slide 2 - Scope:**  
In a program, the scope of a variable indicates how long that variable is
available. This is also known as the lifetime or visibility of a variable.

**Slide 3 - Global Scope:**  
Variables defined at the top level are known as global variables. Once a
variable is defined, it is available on subsequent lines. That variable lives
until the end of the program.

**Slide 4 - Local Scope:**  
Each function has its own local scope. Variables defined as parameters or
within a function live until the function ends. Therefore, variables defined
in one function are not available outside the function. This simplifies the
reading of any function - you only need to worry about things defined in the
function itself.

**Slide 5 - Returning Values:**  
Functions return values, not variables. A variable has a value, so when you
write a statement like the one shown, you are returning the variable's value,
not the variable itself. The variable disappears after the function ends, so
returning the value is the only way to make it available. Any global variables
with the same name are actually unrelated to the variable inside the function.

**Slide 6 - Global Variables Are Bad:**  
It is technically possible to read a global variable inside a function.
However, you should not do so. Every time you refer to global variables, your
program becomes more complicated and you have to think about multiple levels
of scope. This may work out okay in smaller programs, but causes huge problems
as you start writing longer programs. Whenever you feel the urge to use a
global variable, stop and reconsider.

**Slide 7 - Scope Rule of Thumb:**  
Here is a simple pair of rules for working with scope: Variables inside a
local scope should not be used outside that scope. Variables outside a local
scope should not be used inside that scope. Keeping these two rules in mind
will avoid many headaches. Okay, are Global Variables really bad? Let's
discuss further: http://wiki.c2.com/?GlobalVariablesAreBad

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Variables created inside a function cannot be used outside the function, and
variables created outside a function should not be used within.