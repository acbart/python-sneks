This class gives a more formal introduction to Strings. Although we covered
Strings briefly back when we learned about types, now we're studying them in
more depth.

###  &icon-check-plus; Objectives

  1. Define the concept of a string
  2. Create a string literal
  3. Create a triple-quoted string
  4. Incorporate escape characters into a string

###  &icon-quiz; Activities

  * [#15) Lesson: Strings](#video)
  * [#15) Quiz: Strings](https://vt.instructure.com/courses/66476/assignments/356617)
  * [#15) Programming: Strings](https://vt.instructure.com/courses/66476/assignments/356662)

###  &icon-educators; Lesson

Download Slides:
[Strings.pptx](https://vt.instructure.com/courses/66476/files/5919835/download?verifier=iire6InLsL4gYoNm3mTutFmmUHuG0VMW9wXBcPv4&wrap=1
"Strings.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="String Operations"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/IQKYJ4weBfM?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Strings:**  
Let's learn about Strings.

**Slide 2 - Purpose:**  
Strings are how we put text data into a computer. Any text data can be a
string: names, words, books, web sites.

**Slide 3 - Characters:**  
Strings are made up of letters, numbers, and symbols. We call these things
"characters".

**Slide 4 - The name String:**  
Think of a String like a necklace, where each bead has a character on it. We
"string together" letters. The single or double quotes are knots at the end
that tie the letters off.

**Slide 5 - Quotes:**  
Strings are represented with quotes. You can use either double quotation marks
or single quotation marks. However, if you start a String with double, you
must end with double. If you start with single, you must end with single. The
reason there are two kinds is to make it easier to create strings like the
below

**Slide 6 - Escape Characters:**  
So how do you have a string with both single and double quotes in it? You can
use special combinations of characters called "escape characters". By putting
a back-slash "\" before a character, you create a special character. Check out
the example below here, where we have escaped the double quote character.

**Slide 7 - Other Escape Characters:**  
There are actually many kinds of escape characters. Here are two more you may
see. \n is a new line (like pressing enter) \t is a "tab" character, or
multiple spaces (like indenting a paragraph)

**Slide 8 - Numbers and Strings:**  
It's a little confusing, but you can put a number in quotes. However, this
means that you have a String and not an Integer. The difference becomes very
obvious when you try to add things together. "1" + "2" is "12", instead of 3.
Python is very strict about the differences between Numbers and Strings.

**Slide 9 - Variables and Strings:**  
Some people confuse Variables and Strings, but they are very different.
Remember, variables hold values. Strings are just a type of value that
represent text.

**Slide 10 - Triple Quoted Strings:**  
Rarely, you have to put a huge amount of text into your program. The best way
to do so is to use "triple quoted strings". The syntax is simple: you start
and end the chunk of text with three quote marks. It doesn't matter if they
are single or double quotes, as long as it starts and ends the same.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

  * Automate the Boring Stuff: [Chapter 6](https://automatetheboringstuff.com/chapter6/) until 'Useful String Methods'
  * Coding for Beginners: Pages 112-113
  * How to Think like a Computer Scientist: [9.1](http://interactivepython.org/runestone/static/thinkcspy/Strings/StringsRevisited.html)-[9.4](http://interactivepython.org/runestone/static/thinkcspy/Strings/IndexOperatorWorkingwiththeCharactersofaString.html)

###  &icon-flag; Summary

You should now feel comfortable with representing a string in your computer,
and then manipulating them.