In this lesson, you will learn functions are evaluated for correctness using
Unit Tests. Unit tests are a battery of known inputs and outputs for a
function that can be run conveniently to verify assertions about the program.

###  &icon-check-plus; Objectives

  1. Explain how functions are tested for correctness.
  2. List advantages of using unit tests
  3. Intepret a failing unit test
  4. Describe the limitations of unit tests

###  &icon-quiz; Activities

  * [#21) Lesson: Unit Tests](#video)
  * [#21) Quiz: Unit Tests](https://vt.instructure.com/courses/66476/assignments/356597)
  * [#21) Programming: Unit Tests](https://vt.instructure.com/courses/66476/assignments/383583 "#21\) Programming: Unit Tests" )

###  &icon-educators; Lesson

Download Slides: [Unit
Tests.pptx](https://vt.instructure.com/courses/66476/files/5919796/download?verifier=wmI73BknaMdDGjnzXKi1bbmGUbujSBXFqX10qJow&wrap=1
"Unit Tests.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Unit Tests"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/upzTwaVNZzs?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Unit Tests:**  
Let's learn about Unit Tests.

**Slide 2 - Unit Tests:**  
Once you've created a function, how do you know if it is correct? You could
carefully read over the function, but you might miss something. Instead,
programmers use collections of Unit Tests to determine if their code works as
expected. Unit testing is an important professional practice to help you find
problems early, facilitate changes down the road, and make it easier to glue
together pieces of code.

**Slide 3 - Example Unit Test:**  
A unit test is pretty simple: given a fragment of code like a function, run
the function for a known input and compare it to a known output. For example,
consider this function that converts feet to inches. Below it is a collection
of 5 possible inputs and the 5 expected outputs. These are our unit tests.

**Slide 4 - Representative Cases:**  
A tricky part of making unit tests is thinking of appropriate test cases. The
goal is to cover many possible scenarios, while writing the minimum number of
cases. In our conversion function before, we tried it with a small positive
number, a decimal number, a negative number, a large number, and zero. These
are all representative cases

**Slide 5 - Failing Unit Tests:**  
When a unit test fails, it should report the actual and expected values, so
that the programmer can then debug their program. If you only try a function
with one output, you might think that the function is correct. But until you
run unit tests, you shouldn't believe that. Of course, unit tests are not
conclusive either, they are merely evidence to support the hypothesis that
your code is correct.

**Slide 6 - Passing Unit Tests:**  
The larger your program, the more important it is to unit test individual
pieces. However, unit tests are also helpful as you learn the basics. Every
program you write in this course will be unit tested, which means that we will
try running your program against many inputs and outputs. Just because your
program appears to give the right output, you must pass all the unit tests!

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Unit tests are used to ensure that a function is correct.