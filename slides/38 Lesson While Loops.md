In this lesson, you will learn about a new kind of loop called WHILE loops.
These loops are somewhat different from FOR loops, and in fact act more like
IF statements. Although WHILE loops are common in other languages, they are
less useful in Python, so we will not use them very much.

###  &icon-check-plus; Objectives

  1. Compare and contrast the For loop and While loop
  2. Define a While loop
  3. Determine if a situation requires a While loop
  4. Write code that involves condition based iteration
  5. Define control structure
  6. Identify control structures in code
  7. Describe the impact of various control structures on the sequence of a program.
  8. Nest control structures

###  &icon-quiz; Activities

  * [#38) Lesson: While Loops](#video)
  * [#38) Quiz: While Loops](https://vt.instructure.com/courses/66476/assignments/356612)
  * [#38) Programming: While Loops](https://vt.instructure.com/courses/66476/assignments/356678)

###  &icon-educators; Lesson

Download Slides: [While
Loops.pptx](https://vt.instructure.com/courses/66476/files/5919810/download?verifier=yHUNywHWwfNZF7jknaF2DclUxKRVsdPfvwjOCUas&wrap=1
"While Loops.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="While Loops"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/BOebf9j44V4?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - While Loops:**  
Let's learn about While Loops.

**Slide 2 - Another Kind of Iteration:**  
FOR loops allow us to iterate through each element of a list. They are the
most common form of iteration in Python. However, there is another kind of
iteration, called While loops.

**Slide 3 - Syntax:**  
Notice how the syntax for a WHILE loop is similar to that of an IF statement.
We have the word WHILE, followed by a condition, ending with a colon. Then we
can have any number of statements inside the body. Remember that this body,
like a FOR loop or an IF statement, is indented with 4 spaces.

**Slide 4 - Like IF Statements:**  
WHILE statements are actually very similar to IF statements. However, instead
of executing once or none, they will execute repeatedly until the condition is
true.

**Slide 5 - Tracing the Flow:**  
When a While loop is executed, the program follows a similar looping behavior
as a FOR loop. Here we can see that behavior in a WHILE loop to count down
from 10. The program tests the condition, and if it is true, then it moves
through each statement in the body. Then, it returns to the top and tests the
condition again. If it is still, true, it repeats the previous loop.
Otherwise, it skips to the end of the WHILE body.

**Slide 6 - Looping Forever:**  
A tricky thing about WHILE loops is that it is easy to loop forever by
accident. Consider the code below. Because the variable " count_down " is only
ever increasing, it will never reach zero and the loop never ends.

**Slide 7 - While Loops Are Awful:**  
The FOR loop is almost always superior to the WHILE loop, because they
terminate after the list is procesed ; it is almost impossible to loop
infinitely. Most of the time, you should use a FOR loop instead of a WHILE
loop. As an example, consider the counting code shown before. Instead, that
can be efficiently replaced with a FOR loop that calls the "range" function,
which consumes a integers and produces a list of integers counting up to that
number.

**Slide 8 - User Input Loop:**  
One of the very few cases for a WHILE loop is useful is dealing with repeated
user input. For instance, the Read-Evaluate-Print-Loop that powers a command
line like IPython uses a While loop. The pattern shown here is one way to
handle repeated user input. This repeatedly asks for words until the string
"EXIT" is given, at which point it will exit the loop.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

The WHILE loop repeatedly performs a body of actions until its condition is no
longer true. In this way, they are very similar to an IF statement that loops
back on itself.