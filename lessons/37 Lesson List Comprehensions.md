In this lesson, we will learn how to create list comprehensions. List
comprehensions use FOR Loops to conveniently create a list.

###  &icon-check-plus; Objectives

  1. Create a list using a list comprehension
  2. Create a list using a list comprehension and filtering
  3. Identify the advantage of a list comprehension over other forms of list creation
  4. Identify the drawback of using a list comprehension over regular FOR loops.

###  &icon-quiz; Activities

  * [#37) Lesson: List Comprehensions](#video)
  * [#37) Quiz: List Comprehensions](https://vt.instructure.com/courses/66476/assignments/356614)
  * [#37) Programming: List Comprehensions](https://vt.instructure.com/courses/66476/assignments/356677)

###  &icon-educators; Lesson

Download Slides: [List
Comprehensions.pptx](https://vt.instructure.com/courses/66476/files/5919833/download?verifier=d34ZrzVEyR21AUwUFKvmYDcSqmDjTApimZZfRP5m&wrap=1
"List Comprehensions.pptx" ){: .instructure_file_link
.instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="List Comprehensions"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/UxeeoHeOxSI?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - List Comprehensions:**  
Let's learn about List Comprehensions

**Slide 2 - Transforming a list:**  
Frequently, we want to create a new list based on an old list. You could use
the Transform pattern that we learned previously, as shown here where we
double each element of a list. However, we will now learn a much more
convenient way to do the same thing.

**Slide 3 - List Comprehensions:**  
A List Comprehension allows you to create a list from an old list using a FOR
loop. You can see the syntax here. We begin by placing square brackets on
either end of the expression. Then, we'll put an expression followed by the
"for item in old_list " syntax that we used with for loops. Notice that we no
longer use a colon. Also notice that we no longer need the word append.

**Slide 4 - The Element:**  
With a FOR loop, you can put multiple statements inside the body of the loop.
With a comprehension, you can only put a single expression at the start of the
comprehension. This expression is the "element", which will be used to create
the new list. Notice how the element expression uses the iteration variable.

**Slide 5 - Examples:**  
Here we see a list comprehension to make a list of strings all lowercase. Each
word becomes lowercase, and placed into a new list.

**Slide 6 - Drawbacks:**  
Although a list comprehension is more convenient than a full FOR loop, you
should remember they are not quite the same. A `for` loop has a body of
statements, which means it can do more than one thing inside itself. A List
Comprehension only has a single expression, which means it cannot do more than
one thing. Further, the list comprehension can only have expressions, not
perform statements like an assignment. Consider the example below, where we
are calculating a sum of a list of prices and also transforming the list of
prices. We cannot do the same thing with a List Comprehension, because it
requires multiple actions, some of which are also statements!

**Slide 7 - Filtering Comprehensions:**  
There's one more thing to know about List Comprehensions: you can add an IF
clause, to optionally filter items. It may be a little strange to see the
syntax, but the idea is pretty straightfoward . Create a new list based on an
old; when creating a new element, only keep that element if the conditional is
true. Note that in the example shown here, the resulting list will only be two
elements long: the 5 is filtered out, because the old value is 5, and we only
double the new value if the conditional was true.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

List comprehensions are a type of expression similar to a FOR loop, but are
explicitly for creating new lists. They are very convenient shorthand for
creating lists.