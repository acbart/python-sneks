In this lesson, we will learn more about lists. Specifically, the differences
between lists and strings. Strings have some important differences from lists,
but also some shared behavior.

###  &icon-check-plus; Objectives

  1. Iterate through a string
  2. Process a String with a FOR loop
  3. Differentiate between a list and a string

###  &icon-quiz; Activities

  * [#35) Lesson: Lists and Strings](#video)
  * [#35) Quiz: Lists and Strings](https://vt.instructure.com/courses/66476/assignments/356637)
  * [#35) Programming: Lists and Strings](https://vt.instructure.com/courses/66476/assignments/356676)

###  &icon-educators; Lesson

Download Slides: [Lists and
Strings.pptx](https://vt.instructure.com/courses/66476/files/5919835/download?verifier=iire6InLsL4gYoNm3mTutFmmUHuG0VMW9wXBcPv4&wrap=1
"Lists and Strings.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Lists and Strings"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/YHvrPZ_Rnm0?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Lists and Strings:**  
Let's learn more about Lists and Strings

**Slide 2 - Processing a String:**  
Lists and Strings are somewhat similar, since they are both a sequence of
things. Strings are sequences of characters, but Lists can be a sequence of
anything. The key idea is that both Strings and Lists are sequences, which
means that you can iterate over them with a FOR loop. When you iterate over a
list, you get each element. When you iterate over a string, you get each
character.

**Slide 3 - Using the split() method:**  
Often, instead of processing a list character-by-character, we want to process
it word-by-word, or by some other chunking of characters. To make this easy,
strings have a method named split. Split is an awesome method because it is
easy to use.

**Slide 4 - For Loop and Split:**  
As you can see below, after we have split a string, it is easy to loop over
each word. In this example, we separate each author to print them
individually.

**Slide 5 - Splitting on Characters:**  
If you do not pass anything to split, then it splits on any kind of whitespace
- spaces, tabs, new lines. Sometimes, we want to split on other characters.
You can pass a string as an argument to split on a different character.

**Slide 6 - Input/Split/Loop:**  
Here is a useful pattern. You take a comma-separated string from the user,
split the elements, and process each one in turn. Notice how we can use this
to process a string of numbers by converting them using the " int " function.
Study each statement of this pattern carefully, and make sure you understand
it.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

FOR Loops are not just useful for lists - they can also be used with Strings
and other sequence types.