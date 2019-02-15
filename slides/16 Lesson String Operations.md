This lesson teaches basic operations on Strings. We'll learn how to manipulate
and extract information about those strings.

###  &icon-check-plus; Objectives

  1. Combine two strings
  2. Compare two strings
  3. Subscripting a character from a string
  4. Subscripting a range of characters from a string

###  &icon-quiz; Activities

  * [#16) Lesson: String Operations](#video)
  * [#16) Quiz: String Operations](https://vt.instructure.com/courses/66476/assignments/356601)
  * [#16) Programming: String Operations](https://vt.instructure.com/courses/66476/assignments/356663)

###  &icon-educators; Lesson

Download Slides: [String
Operations.pptx](https://vt.instructure.com/courses/66476/files/5919843/download?verifier=y8kclICmXESoizIq2IhVYEjwPrnea9Ghk3wcfNme&wrap=1
"String Operations.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="String Operations"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/OgWBaU9FZTE?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - String Operations:**  
Let's learn about String Operations.

**Slide 2 - Addition:**  
Like numbers, you can add two strings together. This puts them side by side
ina single new string. This is sometimes called "Concatenation".

**Slide 3 - Comparing Strings:**  
You can test if two strings are equal, not equal, or even compare them using
less than and greater than. This measures which ones come first in the
alphabet.

**Slide 4 - Membership in Strings:**  
There's another test you can check with Strings: using the "in" operator. This
simply checks whether the first string appears in the second. You can also use
the "not in" operator to test the opposite.

**Slide 5 - Subscripting:**  
Subscripting is one of the more powerful and more complex features of strings.
When we *subscript* a string, we extract one or more characters from the
string.

**Slide 6 - Subscript Syntax:**  
We can subscript a string value or variable by using square brackets. Notice
the key components: On the left is the name of the variable or the string
literal value. Next we have an opening square bracket. Then, we have a number,
which is called the index. Finally, we end with a closing square bracket.

**Slide 7 - Starting at 0:**  
Here's a weird thing: computers start counting at 0, not 1. So if you want the
first character from the string, you need to write 0 instead of 1. There are
mathematical reasons why computers work this way, but ultimately it ends up
being more convenient, once you get used to it. But you can see in this string
that, starting from 0, every character (including the space) is assigned an
index. I can get out the second "r" by using index 3, and the capital P by
using index 6.

**Slide 8 - Subscripting Multiple Characters:**  
It wouldn't be too useful to only grab out one character at a time. So you can
actually grab out more than one by using the subscript range syntax. Inside
the square brackets, you put a pair of numbers separated by a colon. The first
number is the starting index, and the second number is the closing index.

**Slide 9 - Negative Subscript Indices:**  
If you use negative numbers as subscript indexes, you can work from the back
of the list. If you use -1, then you get the last character. You can combine
positive and negative numbers in your indexes. To go from the start or the
end, simply leave the number missing.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

  * Automate the Boring Stuff: [Chapter 6](https://automatetheboringstuff.com/chapter6/) until 'Useful String Methods'
  * Coding for Beginners: Pages 112-113
  * How to Think like a Computer Scientist: [9.1](http://interactivepython.org/runestone/static/thinkcspy/Strings/StringsRevisited.html)-[9.4](http://interactivepython.org/runestone/static/thinkcspy/Strings/IndexOperatorWorkingwiththeCharactersofaString.html)

###  &icon-flag; Summary

Strings can be manipulated according to their own rules and operations,
distinct from integers and booleans.