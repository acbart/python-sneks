In this lesson, you will learn about specific concrete patterns for how to use
dictionaries. This builds on the previous lesson about dictionaries, showing
some general ways that you can use Dictionaries.

###  &icon-check-plus; Objectives

  1. Use a dictionary to look up data
  2. Use a dictionary as a struct/record
  3. Use a dictionary to keep track of occurrences
  4. Use dictionary access to access a variable key

###  &icon-quiz; Activities

  * [#40) Lesson: Dictionary Patterns](#video)
  * [#40) Quiz: Dictionary Patterns](https://vt.instructure.com/courses/66476/assignments/356650)
  * [#40) Programming: Dictionary Patterns](https://vt.instructure.com/courses/66476/assignments/356681)

###  &icon-educators; Lesson

Download Slides: [Dictionary
Patterns.pptx](https://vt.instructure.com/courses/66476/files/5919820/download?verifier=NQlJxLuSboFEwoJPIvynmh80pRGgalqPqDceJaxl&wrap=1
"Dictionary Patterns.pptx" ){: .instructure_file_link
.instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Dictionary Patterns"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/nMJKO_fij9c?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Dictionary Patterns:**  
Let's learn about Dictionary Patterns.

**Slide 2 - Using Dictionaries:**  
Dictionaries are very useful for a broad number of applications. However, it
can be tricky to understand how to use them. In this lesson, you will see some
common patterns for how to use Dictionaries.

**Slide 3 - Lookup Pattern:**  
Dictionaries can be used to quickly convert one value into another. Consider
the example here; this dictionary can be used to words to their abbreviation.
Note that this could have also been implemented as a function with an IF
statement. However, if you are only looking up a single value, then the
dictionary will be much easier and faster. Although this example uses strings,
you can really map any type of data to any other type of data in a lookup
dictionary.

**Slide 4 - Record Pattern:**  
With the Record Pattern, dictionaries become a useful way to hold data that
represents a single complex thing. In the example below, we represent a person
using a dictionary with 3 keys. Notice that in this pattern, each key is a
string. The values can be whatever type of data is useful, but they will
always have the same type as other records that represent that complex thing.
By convention, all records meant to represent the same type of real world
thing (like a person) will have the same keys with the same spelling.

**Slide 5 - Counting Pattern:**  
We have previously used the Counting pattern to count the number of
occurrences of an item in a list. But what if we want to count the occurrences
for each possible item in a list, without knowing the items before hand? By
adding in a dictionary, we can do just that. The counting pattern results in a
dictionary of any kind of keys mapped to integers. Notice that dictionary
access can be used to update a value, in addition to getting a value. When the
dictionary access occurs on the left side of an assignment, the value
associated with that key will be replaced. Moreover, you can see that we are
using a variable to access elements, instead of a string literal.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Dictionaries are flexible data structures that can be used in a number of
ways. They can be records to represent complex data, as a lookup tool to
simplify conversions, and as a tool for counting unknown categories of a list
of data.