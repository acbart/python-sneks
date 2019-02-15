This lesson builds on the previous to help you better understand how to define
new functions.

###  &icon-check-plus; Objectives

  1. Use functions to solve problems
  2. Evaluate the name of a function
  3. Extract code into a function
  4. Define functional decomposition

###  &icon-quiz; Activities

  * [#25) Lesson: Function Development](#video)
  * [#25) Quiz: Function Development](https://vt.instructure.com/courses/66476/assignments/356649)
  * [#25) Programming: Function Development](https://vt.instructure.com/courses/66476/assignments/356668)

###  &icon-educators; Lesson

Download Slides: [Function
Development.pptx](https://vt.instructure.com/courses/66476/files/5919795/download?verifier=bHyn684oy0bgZfdGKktJ6D9LwmMuVlQBlW53bO9B&wrap=1
"Function Development.pptx" ){: .instructure_file_link
.instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Function Development"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/inZm1a3HJH0?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Function Development:**  
Let's learn more about Defining Functions.

**Slide 2 - Example:**  
The code below converts a temperature from Fahrenheit to Celsius. This code
has some issues, however. First, the calculation is called multiple times in
the code, which makes it much more likely for a mistake to occur when typing
it. Second, if a mistake does occur, it will be harder to track down in the
offending lines. Third, anyone not familiar with the formula might wonder what
this code is doing. A function will help us with all of these problems.

**Slide 3 - 1) Start the Definition:**  
We begin with the skeleton of a function. In BlockPy , the Function block
generates this function, ready for editing.

**Slide 4 - 2) Name the function:**  
If you cannot name a function, then you probably don't know what it should do.
We know that this function will convert a temperature, so let's call it
convert_temperature . This name is short and has a verb. Notice how I used
underscores to represent spaces, because function names follow the same rule
that variables do.

**Slide 5 - 3) Find Commonalities:**  
You need to identify what is the same and what is different about each call.
Extract out the code that is the same. Here, we've extracted out the
calculation. We could have extracted out the print too, but remember that
printing and returning are different. Usually, functions don't need to print
anything.

**Slide 6 - 4) Parameterize:**  
Notice the blank in the code we extracted. Since the value we converted was
different each time, we need to parameterize it by giving those concrete
values a more general name. In this case, each time it was a temperature in
Fahrenheit, so we'll call this " a_fahrenheit ". We put this new parameter in
the function's header and then use it in the body.

**Slide 7 - 5) Return:**  
The code we've created is meant to go inside the body of the function, but we
have nothing to connect it to yet. Recall that this function should return the
temperature in celsius . Therefore, we need a return block. This gives us the
open connection we need to incorporate the formula we extracted earlier.

**Slide 8 - 6) Call:**  
Finally, we can now call our function in the code. Notice how we connect the
original values as arguments for our function call.

**Slide 9 - Watch the Execution:**  
So what actually happens when you call a function? Let's see it in action.
Notice how the execution jumps BACKWARD when we call a function, and then
returns later. (You can view this yourself: https://goo.gl/TXXaBT)

**Slide 10 - Other Approach:**  
Here, we turned existing code into a function definition and then called the
function. Another common approach is to do the opposite: write the function
call, and then use that to write the function definition. Use whichever order
is more comfortable for you when solving each problem.

**Slide 11 - Functional Decomposition:**  
When writing out a solution, you can use a powerful tool called Functional
Decomposition. The idea is to break a complex problem into easier parts.
Consider the task of going to the store. You could break this long algorithm
into three shorter subtasks, and focus on solving each in turn.

**Slide 12 - Keywords:**  
We have now learned a few keywords: def, return, and pass. In previous
lessons, we learned a few other keywords: and, or, not, and in. Python has a
small set of keywords, and you will eventually learn most of them. An
important detail to remember is that we cannot name variables or functions
using keywords, because Python will get confused by what we are trying to say.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Functions allow us to extract commonly repeated chunks of code.