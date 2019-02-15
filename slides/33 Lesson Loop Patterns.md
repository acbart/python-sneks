This lesson builds further on the lesson from the previous day. There are many
common ways that FOR loops are used, and the best way to learn this looping
structure in general is to learn some core patterns.

###  &icon-check-plus; Objectives

  1. List the common patterns associated with FOR loops
  2. Match a problem with the associated loop pattern
  3. Use the Map pattern of FOR loops to transform a list
  4. Use the Filter pattern of FOR loops to remove elements from a list
  5. Use the Sum pattern of FOR loops to summate a list of integers
  6. Use the Count pattern of FOR loops to count the length of a list
  7. Use the Accumualte pattern of FOR loops to combine elements of a list
  8. Use the Min/Max pattern of FOR loops to find the highest or lowest element of a list
  9. Modify a loop pattern to solve a problem

###  &icon-quiz; Activities

  * [#33) Lesson: Loop Patterns](#video)
  * [#33) Quiz: Loop Patterns](https://vt.instructure.com/courses/66476/assignments/356598)
  * [#33) Programming: Loop Patterns](https://vt.instructure.com/courses/66476/assignments/356675)

###  &icon-educators; Lesson

Download Slides: [Loop
Patterns.pptx](https://vt.instructure.com/courses/66476/files/5919837/download?verifier=RFYeDZ6t4dNVTILnltopeAqWM6SnCQkw8jBPaBqN&wrap=1
"Loop Patterns.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Loop Patterns"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/YzAuki4eTyQ?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Loop Patterns:**  
Let's learn about Loop Patterns

**Slide 2 - Many Patterns:**  
There are so many ways to use For loops. In this lesson, we will review a few
common patterns. These patterns shown here are just starting points. Think of
them as templates that can be adapted and combined to solve more complex
problems.

**Slide 3 - Count Pattern:**  
We have a list of items, and want to know how many there are. A simple
algorithm is, starting with an initial value of 0, to add 1 for each element
we see to a "count" variable. When the loop is finished, the "count" variable
will have the length of the list.

**Slide 4 - Sum Pattern:**  
We have a list of numbers, and want to add them all up. The plus operator can
only take two items at a time, however. Therefore, we add each element one at
a time to a "sum" variable, which is also initialized to 0. As you can see
the, the sum pattern is similar to the Count pattern, except instead of adding
1, we are adding the iteration variable.

**Slide 5 - Accumulator Pattern:**  
The Sum and Count patterns are both more specific examples of the accumulator
pattern. In general, this pattern allows us to start with an initial value and
use any function or operation that takes in two values. This pattern can be
applied to numbers, but it also works for strings, booleans , and even lists.
This process of accumulation is also sometimes known as "reducing" or
"folding" a list.

**Slide 6 - Map Pattern:**  
What happens when we accumulate a list? If we start with an empty list as our
initial value, and append each value one at a time, we end up with a copy of
the original list. As we're appending values, we can also modify them. For
example, you could double each value from the old list, or convert each
temperature from Fahrenheit to Celsius.

**Slide 7 - Filter Pattern:**  
We have a list of numbers, and want to ignore some of them according to a
rule. By embedding an IF statement inside the loop, we can optionally include
or not include elements in our accumulation. The Filter pattern is very
compatible with the other patterns.

**Slide 8 - Min/Max Pattern:**  
The last pattern is used to find the highest or lowest element in a list. At
first, it may appear similar to the Filter pattern, because it uses an IF
statement. However, you can see that instead of comparing each element to a
constant value, the conditional compares each value to the accumulated value.
Using this pattern, the accumulated value (in this case a maximum) will end up
as the highest value in the list.

**Slide 9 - Inside or Outside of the Body:**  
Novices always struggle with what goes inside or outside of a loop body.
Remember, every statement inside the body is executed for each element. Only
put things inside if they should happen for each element. The patterns can
help you keep track of where things go, but ultimately you have to think
critically to know.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

FOR loops are usually used in a few recurring patterns that are useful to
memorize.