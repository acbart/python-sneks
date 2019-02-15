In this lesson, you will learn about FOR loops. The FOR loop allows you to
perform actions on each element of a list, so they go hand-in-hand with lists.
FOR loops are one of the most difficult topics for beginners, so expect to
spend a lot of time with them. However, they are essential for doing useful
things with lists, so you should be sure to learn them.

###  &icon-check-plus; Objectives

  1. Define a For Loop and Iteration Variable for an Iteration List
  2. Construct an Iteration Variable for an Iteration List
  3. Write code that involves iteration over a list value
  4. Write code that involves iteration over a list variable
  5. Identify the type of the iteration variable with respect to the iteration list
  6. Determine if a situation requires a For loop

###  &icon-quiz; Activities

  * [#32) Lesson: For Loops](#video)
  * [#32) Quiz: For Loops](https://vt.instructure.com/courses/66476/assignments/356593)
  * [#32) Programming: For Loops](https://vt.instructure.com/courses/66476/assignments/356674)

###  &icon-educators; Lesson

Download Slides: [For
Loops.pptx](https://vt.instructure.com/courses/66476/files/5919826/download?verifier=p4JvF2E9GS3kfNqwCIHe8HI7mYnss7dagTCeiRey&wrap=1
"For Loops.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="For Loops"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/eEaeXtX4Fv8?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - For LOOPs:**  
Let's learn about For Loops.

**Slide 2 - Doing Things Multiple Times:**  
Observe the code below, which prints out the following 5 numbers. We had to
write a print statement 5 times, once for each number. Surely there's a way
that will let us stop writing the same chunk of code each time? For Loops are
an amazingly useful tool that let us perform an action on each element of a
list.

**Slide 3 - Syntax:**  
Here's how we write a For loop. First, we write the word 'for'. Then we make a
new variable named the iteration variable. We'll come back to this later.
Next, we write the word 'in'. Then, we put the list variable or value that we
want to iterate over. After that, we need to put a colon. Finally, we put any
statements to run inside the body of the loop.

**Slide 4 - The Iteration List:**  
A crucial element of any For loop is the iteration list. This is the data that
we want to iterate over. When the loop executes, each item of the list will be
assigned to the iteration variable in turn. It doesn't matter if the list has
no items, ten items, or a thousand items; Python will still process each one
in turn.

**Slide 5 - The Iteration Variable:**  
One of the hardest things to understand about For loops is the iteration
variable. The iteration variable represents the generalized version of each
item in the list. If you have a list of temperatures, it is "a temperature".
If you have a list of books, it is "a book". By performing operations on this
generalized version of a list item, you can work on the entire list while only
having to think about one element at a time.

**Slide 6 - The Body:**  
Just like an If statement, we can put statements inside of a For loop. Each
statement is indented with four spaces, and each statement will be executed
one-by-one, from top to bottom.

**Slide 7 - The Flow of a For Loop:**  
Previously, we said that a program was like a river, running from the top to
the bottom. If statements made the stream split into two directions. For loops
also make the stream split, but one of the new streams will move back up. This
is the crucial idea, and its why we call it a loop. The program will LOOP
until each element of the list has been assigned to the iteration variable.

**Slide 8 - Tracing a For Loop:**  
Let's look at a loop in practice. Notice how the value of the iteration
variable changes each time we go through the loop again, and the cursor jumps
back up to the start of the loop. This behavior is crucial! (You can view this
yourself: https://goo.gl/yebYBw)

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

The FOR loop performs a body of actions on each element of a list, one at a
time. The body is written to perform the action on a generic iteration
variable that represents each of the elements of the list.