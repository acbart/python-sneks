In this lesson, you will learn about IF statements. These affect the flow of
your program so that you can do different things at different times. In other
words, IF statements make your program smart and adaptable to different
situations.

###  &icon-check-plus; Objectives

  1. Write code that involves nested if statements
  2. Write code with branching conditions
  3. Trace branching control flow
  4. Differentiate between double IFs and the ELIF

###  &icon-quiz; Activities

  * [#29) Lesson: Nesting Blocks](#video)
  * [#29) Quiz: Nesting Blocks](https://vt.instructure.com/courses/66476/assignments/356646)
  * [#29) Programming: Nesting Blocks](https://vt.instructure.com/courses/66476/assignments/356670 "#29\) Programming: Nesting Blocks" )

###  &icon-educators; Lesson

Download Slides: [Nesting
Blocks.pptx](https://vt.instructure.com/courses/66476/files/5919840/download?verifier=VPjUQXaqzTV52NG7ePFmnGHFvK41Qh161im2jrTm&wrap=1
"Nesting Blocks.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Nested Ifs"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/6AaULEfcgv4?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Nesting Blocks:**  
Let's learn about Nesting Blocks.

**Slide 2 - Nesting:**  
You can put IF statements inside of IF statements. We call this "nesting". As
you develop more complex programs, you will do a lot of nesting.

**Slide 3 - Number of Spaces:**  
Whitespace rules can be confusing. Every time you nest a block inside another
block, the body gets indented another 4 spaces. Observe the BlockPy blocks on
the left, and their resulting whitespace on the right.

**Slide 4 - IF and Functions:**  
You can put IF statements inside of functions. In fact, this is both common
and useful. Remember the whitespace rules when this occurs. Each nested block
is another 4 spaces in.

**Slide 5 - What Goes Inside?:**  
It can be difficult to know if something belongs inside or outside of a block.
You must be aware of what you are trying to do with the IF block. Remember:
statements inside the IF block are executed only if the conditional evaluates
to True. Think critically!

**Slide 6 - ELIF block:**  
In addition to the IF and ELSE blocks, there is a third type: ELIF. The ELIF
is exactly equivalent to an ELSE block with an IF inside. However, they are
sometimes used for convenience.

**Slide 7 - Two IFs vs ELSE IF:**  
The following two pieces of code may look similar, but they are quite
different. The code on the left has two IF statements, and both will always be
evaluated and potentially executed. The code on the right has an ELIF
statement, and the second will only be evaluated if the first one evaluates to
false.

**Slide 8 - Unnecessary IF:**  
Two kinds of mistakes are very common with IF statements. The first common
mistake is using an IF statement when a conditional expression is fine on its
own. For example, consider this function definition that returns True if the
parameter is greater than 5, or otherwise returns False. The conditional
expression already evaluates to either True or False, so it was unnecessary to
use an If statement. Instead, you can directly return the result of the
conditional expression, as shown on the right.

**Slide 9 - Unnecessary Test:**  
A second common mistake is to test if a Boolean expression is equal to True.
Although the expression here, "age &gt; 5 == True", reads like it makes sense
in English, it is redundant in Python. "age &gt; 5" already evaluates to
either True or False. If you compare a Boolean value to True, then the result
is the same Boolean value. Nothing is accomplished, you have simply made your
code more complex.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

IF statements allow your program to do different things dependent on boolean
conditions. The body of the IF statement is either executed or not, which
affects the flow of the program.