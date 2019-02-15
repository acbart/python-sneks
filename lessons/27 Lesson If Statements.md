In this lesson, you will learn about IF statements. These affect the flow of
your program so that you can do different things at different times. In other
words, IF statements make your program smart and adaptable to different
situations.

###  &icon-check-plus; Objectives

  1. Define an If Statement
  2. Evaluate a conditional expression
  3. Determine whether a situation requires an If statement
  4. Write code that involves simple if statement
  5. Write code that involves nested if statements
  6. Write code with branching conditions
  7. Trace branching control flow
  8. Differentiate between double IFs and the ELIF

###  &icon-quiz; Activities

  * [#27) Lesson: If Statements](#video)
  * [#27) Quiz: If Statements](https://vt.instructure.com/courses/66476/assignments/356626)
  * [#27) Programming: If Statements](https://vt.instructure.com/courses/66476/assignments/356669 "#27\) Programming: If Statements" )

###  &icon-educators; Lesson

Download Slides: [If
Statements.pptx](https://vt.instructure.com/courses/66476/files/5919829/download?verifier=Rg47k5KzGZuvB4GS2rVnJMEM3DHOmJeWu6v0oeIQ&wrap=1
"If Statements.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="If Statements"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/A76dTMrTJbg?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - IF Statements:**  
Let's learn about If Statements.

**Slide 2 - If Statements:**  
If this is true, then do that. Otherwise, don't do it. That's the core idea of
an IF statement.

**Slide 3 - Purpose:**  
If statements make code smarter. They let you do different things in different
situations.

**Slide 4 - Syntax:**  
There are four parts to an IF statement. First, you have the keyword "IF".
Then, you have the conditional. The conditional is followed by a colon.
Finally, you have the body of the IF statement, indented with 4 characters.

**Slide 5 - Conditionals:**  
You already learned about writing conditionals, but as a reminder,
conditionals are a way to ask questions. Conditional expressions can be
variables, comparisons, functions, combinations of these using AND, OR, and
NOT.

**Slide 6 - Body:**  
The body of an IF statement is a sequence of one or more statements. This body
must be indented with 4 spaces. Anything indented below the IF keyword is said
to be "inside" the IF statement. These indented statements will be executed if
the conditional was evaluates to true. Otherwise, Python will skip right over
them.

**Slide 7 - The "Else" block:**  
IF statements can optionally have an Else body. If the conditional evaluates
to false, then the ELSE will be executed instead of the IF body. The IF body
will literally be skipped over as if it didn't exist . Only one of the two
bodies will be executed!

**Slide 8 - Branching:**  
Think about your program as a flowing stream. Normally it will go from top to
bottom. An IF statement changes that flow, to optionally go around. We call
that behavior branching. Every time you have another IF statement, you have
another two branches.

**Slide 9 - Tracing Branches:**  
We have previously shown how you can make a trace table that follows the
execution of an IF statement. We now have to add an extra column to this
table, to differentiate between steps and lines. With IF statements, it is
possible that a step may skip a line of code. Even though the program shown
below has 6 lines of code, it only has 4 steps! Notice that on lines with IF
statements, we still have a step, but we simply repeat the values unchanged.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

IF statements allow your program to do different things dependent on boolean
conditions. The body of the IF statement is either executed or not, which
affects the flow of the program.