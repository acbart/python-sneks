In this lesson, you will learn how to create functions of your own. Functions
definitions are composed of several key parts, and have very specific syntax.
Once a function is defined, you can call it in your code. Functions
definitions are a complex process, so we will learn more about them in the
next lesson. When you complete this one, you should feel free to continue
directly onto the next one!

###  &icon-check-plus; Objectives

  1. Determine if a situation could benefit from a function
  2. Break down a complex task into multiple function calls
  3. Identify the scope of variables in and outside of a function
  4. Define a function with a return value
  5. Describe the difference between parameters and arguments
  6. Define a function without parameters
  7. Define a function with parameters
  8. Extract a variable from a function into a parameter
  9. Describe the signature of a function

###  &icon-quiz; Activities

  * [#20) Lesson: Defining Functions](#video)
  * [#20) Quiz: Defining Functions](https://vt.instructure.com/courses/66476/assignments/356631)
  * [#20) Programming: Defining Functions](https://vt.instructure.com/courses/66476/assignments/356667)

###  &icon-educators; Lesson

Download Slides: [Defining
Functions.pptx](https://vt.instructure.com/courses/66476/files/5919818/download?verifier=VuhxZzy60BiyStHN7ysMctiv4GrgEwQUw0oA0ZRG&wrap=1
"Defining Functions.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Defining Functions"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/U8z4wMGjDbU?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Defining Functions:**  
Let's learn about Defining Functions.

**Slide 2 - Defining Functions:**  
You can create your own functions in Python. In fact, this is one of the most
powerful features of programming, the ability to create your own functions.

**Slide 3 - Why Functions?:**  
Lets' talk about two major advantages of functions: First, they allow us to
reuse code. Second, they allow us to debug a chunk of code in isolation from
the rest of the program.

**Slide 4 - Definition Syntax:**  
To create a new function, you use the "def" keyword, which stands for
"define". As you can see, you write "def", the name of the function, an open
parentheses, each of the parameters separated by commas, and a colon. This
line is called the header. Then, you write each line of the body of the
function below, indented 4 characters.

**Slide 5 - Function Body:**  
When you call a function, you are executing the code stored in the "Body" of
the function. Everything "inside" the body should be indented 4 spaces. In the
block version, this is shown visually with the bar on the left. The body can
be one or more lines long.

**Slide 6 - Pass:**  
Sometimes, we want to define a function without writing its body just yet. We
use a special statement named "pass" to fill in the body until we're ready to
write it. Pass is a very special statement: it does absolutely nothing but
take up space. If we didn't put the word pass there, Python would crash with a
syntax error.

**Slide 7 - Tricky Colons:**  
A number of statements in Python require colons at the end. Functions require
colons at the end of the header. One of the most common mistakes people will
make is to forget the colon.

**Slide 8 - Naming a function:**  
Naming a function is just like naming a variable. The same rules even apply:
you may only use letters, numbers, and underscores, and it cannot start with a
number. Choose the name of the function based on what it does at a high level
- typically it should be a verb.

**Slide 9 - Calling Your Functions:**  
After you've defined a function, you can use it. Again, we combine the name of
the function with parentheses.

**Slide 10 - Parameters:**  
When you define a function, you can choose to add in parameters. These
parameters will take on the value of the arguments when the function is
called. This can be very tricky to understand.

**Slide 11 - Parameters and Values:**  
Remember, variables are passed into a function call as values. When you
manipulate the value of the parameter, you are NOT changing the original
variable. That means that the code below prints 5 instead of 0.

**Slide 12 - Return:**  
When defining a function, you can make it return a value. Most functions
return some kind of value. We make Python return values using the "return"
statement.

**Slide 13 - The Effect of Returning:**  
When your function returns something, the calling block will change its shape.
This connects to the earlier ideas about expressions and statements. When it
comes to functions, returning values make functions behave as expressions
instead of statements.

**Slide 14 - Returns Go in Functions:**  
Return statements can only be placed INSIDE of a function definition. BlockPy
will fuss at you when you try to do otherwise. It is impossible to have a
return outside of a function.

**Slide 15 - Print vs. Returning:**  
Printing and returning are two *very* different things, although that may seem
confusing. Printing is how we write stuff to the console, while returning is
used to get data out of functions. When you return a value, you might store it
in a variable and use it later or as part of an expression. The print function
does not return anything - instead it returns the special value None.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Function definitions have a body of code and are described by their header.
Creating functions is necessary for building up programs of scale.