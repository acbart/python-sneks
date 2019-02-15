In this lesson, you will learn about how any expression can be used in an If
statement's conditional expression, in an idea called Truthiness.

###  &icon-check-plus; Objectives

  1. Define the concept of Truthiness
  2. Evaluate a conditional expression

###  &icon-quiz; Activities

  * [#28) Lesson: Truthiness](#video)
  * [#28) Quiz: Truthiness](https://vt.instructure.com/courses/66476/assignments/356647)

###  &icon-educators; Lesson

Download Slides:
[Truthiness.pptx](https://vt.instructure.com/courses/66476/files/5919804/download?verifier=ks0KuZiCjkgzLZZtn0izQZBK8r6hbeYx5A8phAko&wrap=1
"Truthiness.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Truthiness"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/Hiifw2fLJ4M?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Truthiness:**  
Let's learn about Truthiness.

**Slide 2 - Truthiness:**  
Unlike some languages, Python does not require that IF statements have boolean
expressions in their conditional. This may seem surprising, but it is actually
an extremely convenient feature named Truthiness. The idea is that any
expression, whether it is an integer, string, boolean , or otherwise, can be
evaluated in a conditional.

**Slide 3 - Type Truthiness:**  
Any expression can be evaluated as a conditional according to the rules of
Truthiness. How it is evaluated depends on its type.

**Slide 4 - String Example:**  
Let's look at a simple example, where we take some input from a user. If the
user entered an empty string, then we'll print out a different message.

**Slide 5 - Unnecessary Comparisons:**  
When you need to check if a string is not empty, or a number is not 0,
truthiness is the way to go. Notice how each of the following can become much
more concise and clear.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Any expression can be used as a conditional expression. Succinctly, any zero
or empty value is considered false, and non-zero/non-empty values are
considered true.