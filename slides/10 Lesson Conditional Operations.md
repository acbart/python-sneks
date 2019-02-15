In this lesson, you will learn about how to create logical expressions. In
other words, how you use logic when programming.

###  &icon-check-plus; Objectives

  1. Identify the type of a conditional expressions
  2. Describe the limitations of the basic conditional operators with regards to their number of parametsr
  3. Write an equivalency expression using different equality operators
  4. Write a complex conditional with logic operators
  5. Simplify a boolean equivalency check
  6. Write a logical expression that uses AND, OR, NOT

###  &icon-quiz; Activities

  * [#10) Lesson: Conditionals](#video)
  * [#10) Quiz: Conditionals](https://vt.instructure.com/courses/66476/assignments/356606)
  * [#10) Programming: Conditionals](https://vt.instructure.com/courses/66476/assignments/356658)

###  &icon-educators; Lesson

Download Slides:
[Conditionals.pptx](https://vt.instructure.com/courses/66476/files/6117687/download?verifier=nPSfvbsnkzlCSbdZtt25693w3AYV8yy8pSdklLDT&wrap=1
"Conditionals.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Conditional Operations"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/2BuUxKZWCN4?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Conditionals:**  
Let's learn about Conditionals.

**Slide 2 - Purpose:**  
One of the major reasons that programs are useful is because they can do
different things depending on their inputs. To be able to make these
decisions, we need to be able to write "conditional expressions". Think of
these as a question.

**Slide 3 - Comparison Operators:**  
Often, we want to know about the relationship between two numbers. For this,
we use the comparison operators. Each of these operators takes two numbers and
returns either True or False.

**Slide 4 - == (Equal Operator):**  
Okay, this is gonna sound weird, but in Python we use two equal signs to test
for equality. Do not use one equal sign, that means something different.

**Slide 5 - != (Not equal operator):**  
This will be even weirder. In Python, to test if two things are NOT equal, we
use an exclamation mark and an equal sign.

**Slide 6 - , &gt;= (Greater and Less Than):**  
There are four other operators: The less than operator, the greater than
operator, the less than or equal to operator, and the greater than or equal to
operator.

**Slide 7 - Returning True or False:**  
I said before that the operators return either True or False. Mentally imagine
the result of these operations being replaced by True or False. If you print
the value, it will literally be True or False.

**Slide 8 - Boolean Operators:**  
In the same way we can add and subtract numeric expressions together, we can
also combine booleans expressions together. There are three operators for
this: And, Or, and Not

**Slide 9 - And:**  
And returns True if both the left and right expressions are True.

**Slide 10 - Or:**  
Or returns True if either the left or right expressions are True.

**Slide 11 - Not:**  
Not returns True if the expression is False. Unlike AND and OR, the NOT
expression only takes in a single value.

**Slide 12 - Nesting Conditionals:**  
You can connect conditionals into fairly complex expressions, just like you
could with math.

**Slide 13 - Conditionals Are Not Distributive:**  
A common beginner mistake is to think that you can distribute conditionals.
You might think that the code shown here asks if the number 5 is less than 1
or less than 2. But the "or" operator makes the 2 evaluated separately. To
properly ask this question, you need to write the statement below, with the
less than operator used a second time.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

  * Automate the Boring Stuff: [Chapter 1, still the first half](https://automatetheboringstuff.com/chapter1/) ; it's interesting how fast they blaze through this.
  * Coding for Beginners: Pages 36-48
  * How to Think like a Computer Scientist: [2.7](http://interactivepython.org/runestone/static/thinkcspy/SimplePythonData/OperatorsandOperands.html) and [2.9](http://interactivepython.org/runestone/static/thinkcspy/SimplePythonData/OrderofOperations.html)

###  &icon-flag; Summary

Logical operators like &gt;, ==, and "or" can be used to combine any kind of
values to ask True/False questions.