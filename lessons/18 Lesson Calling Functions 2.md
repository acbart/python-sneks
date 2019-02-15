In this lesson, you'll learn more about calling functions and methods. In
particular, you will learn how to read documentation about built-in functions
that you can use. You will also learn how to nest, chain, and combine
functions and methods.

###  &icon-check-plus; Objectives

  1. Interpret documentation for a function
  2. Use a function based on its documentation
  3. Distinguish between Parameters and Arguments
  4. Nest a function call inside another function call
  5. Chain a method onto another method
  6. Combine functions, methods, and operators into a complex expression

###  &icon-quiz; Activities

  * [#18) Lesson: Calling Functions 2](#video)
  * [#18) Quiz: Calling Functions 2](https://vt.instructure.com/courses/66476/assignments/356648)
  * [#18) Programming: Calling Functions 2](https://vt.instructure.com/courses/66476/assignments/356665)

###  &icon-educators; Lesson

Download Slides: [Calling Functions
2.pptx](https://vt.instructure.com/courses/66476/files/5919812/download?verifier=hnbVBpMLjOygruVb7uRWx020dUNHYfyehP0Bz5bK&wrap=1
"Calling Functions 2.pptx" ){: .instructure_file_link
.instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Calling Functions 2"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/DEKAWU12AAU?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Calling Functions 2:**  
Let's learn more about Calling Functions.

**Slide 2 - Built-in Functions:**  
Python has many, many built-in functions. You could never learn them all in
this course. You will learn a few, but it's far more important that you learn
how to learn more about functions.

**Slide 3 - Learning about a Function:**  
Good programmers create documentation for their functions. Documentation is
extra information about a function that makes it clear how it works. There are
many ways to write documentation, but they usually have a few things in
common.

**Slide 4 - Function Documentation:**  
You should look for five major parts. The function's name, its parameters, its
return value, its description, and examples how to use the function.

**Slide 5 - Parameters and Arguments:**  
The Arguments that are passed into a function are also known as Parameters.
Parameters are the formal names that describe those arguments. In the example
here, the arguments are 3 and 10. The documentation tells us that the
corresponding parameters are length and width.

**Slide 6 - Nesting Function Calls:**  
A common task is to nest function calls inside of other function calls. This
means that return value of the inner function becomes the argument of the
outer function.

**Slide 7 - Chaining Methods:**  
When you need to call methods on the same string variable or value, it's a
little different. You will repeat the period, name, and parentheses each time.
In this example, we invoke the title() method on the string "hello world", and
then the count() method. By placing them side-by-side, you can "chain" the
results from left to right.

**Slide 8 - Functions, Methods, and Operators:**  
Since calls are just another expression, you can freely combine them with each
other. Observe the code show, where we combine string addition, a string
method call, and a function. The result of the entire expression is stored
inside this new " string_length " variable. Notice the order of execution,
this can be tricky to follow!

**Slide 9 - Input/Output:**  
You already know two functions: Print is a function that takes in arguments
and writes to the console. Input is a function reads from the console and
returns it as a string value. These two functions are strange, because they
have side effects. The Input function puts a textbox on the console, and the
print function writes text to the console.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Python comes with a huge number of built-in functions and methods. Programmers
learn how to use these by referring to documentation. In practice, functions
are often called in combination with other functions, methods, and operations.