In this lesson, you will learn how Python reports problems with your program,
and how to respond to those errors.

###  &icon-check-plus; Objectives

  1. Explain an error message for different types of errors
  2. Recall the similarity in the terms "Error" and "Exception"
  3. Track down the offending line of an error message
  4. Choose an appropriate solution to the error message
  5. Track down the offending line of an error message in a called function of an external module

###  &icon-quiz; Activities

  * [#14) Lesson: Errors](#video)
  * [#14) Quiz: Errors](https://vt.instructure.com/courses/66476/assignments/356608)
  * [#14) Programming: Errors](https://vt.instructure.com/courses/66476/assignments/356661)

###  &icon-educators; Lesson

Download Slides:
[Errors.pptx](https://vt.instructure.com/courses/66476/files/5919821/download?verifier=kRrBpfDlEi6at3qfVRAQY1R5XOn2zdeC2QAMQLyN&wrap=1
"Errors.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Error Messages"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/VoD-XfiW5V0?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Errors:**  
Let's learn about Errors.

**Slide 2 - Purpose:**  
When something goes wrong with your program, Python will give you an error
message. These messages are meant to help you find where your error is and
what kind of error it is.

**Slide 3 - Types of Error Messages:**  
Python has many, many error messages. It can take a long time to learn them
all. When you encounter an error message you are unfamiliar with, you should
first read and think about the message. If you are not sure what it means, you
should look up the error's meaning in the documentation. Then, you can debug
your program.

**Slide 4 - Terminology:**  
Just a minor point of terminology. Errors are sometimes referred to as
"Exceptions". They're not quite identical, but for our purposes they might as
well be.

**Slide 5 - Identify the error type:**  
Let's imagine that we ran some code, and encountered an error message. In the
bottom left of the error message, you can see the type of error. In the
example here, you can see that we have a " TypeError ". After the error type,
there is usually some further description of the error.

**Slide 6 - Find the Line:**  
It can be tricky to read, but the error message should also identify WHERE the
error occured . Of course, sometimes the error is actually caused by code on a
previous line. You will have to think very critically about whether the error
message is correct.

**Slide 7 - Common Errors: :**  
Let's look at a few common errors. First, here is a NameError . A NameError
comes up when you try to reference a variable that does not exist yet.
Sometimes, you mispelled the name of the variable. Sometimes, you have not
initialized the variable. Sometimes, you initialized the variable, but you did
so AFTER its first usage. In this case, there is a typo in the name "student
grade".

**Slide 8 - Common Errors: :**  
Another common error is the TypeError , which occurs when you use an operator
incorrectly. For example, adding together a string and a number is not
allowed. When you read the error message that is produced, it will describe
what went wrong. Here, it says that we attempted to concatenate (which means
combine) a string and an integer.

**Slide 9 - Common Errors: :**  
A syntax error means that you broke Python's rules of spelling, grammar, and
punctuation. There are many ways to break a programs' syntax. Usually, Python
is very good at suggesting where the error is. Still, sometimes it can be very
tricky to track down a SyntaxError .

**Slide 10 - Debugging Errors:**  
We'll learn some more techniques to help you fix your broken problems in the
coming weeks. For now, think critically about the errors you receive. When you
see one you don't understand, you should ask "What does this error message
mean?" instead of "What is wrong with my program?"

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

  * Automate the Boring Stuff: Not really covered.
  * Coding for Beginners: Pages 32-33
  * How to Think like a Computer Scientist: [Chapter 3](http://interactivepython.org/runestone/static/thinkcspy/Debugging/toctree.html)

###  &icon-flag; Summary

When Python encounters a problem in your program, it raises an error message.
This error message can be read to better understand what went wrong with your
program.