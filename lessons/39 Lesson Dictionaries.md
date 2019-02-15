In this lesson, you will learn about a new composite data type named
Dictionaries. Dictionaries allow us to store more varied kinds of data than
lists, and make it extremely convenient to get an element by a key.

###  &icon-check-plus; Objectives

  1. Create a dictionary literal
  2. Describe the subtypes of a dictionary
  3. Iterate through a dictionary using .keys(), .values(), and .items()
  4. Use dictionary access to access a literal key
  5. Test membership within a dictionary

###  &icon-quiz; Activities

  * [#39) Lesson: Dictionaries](#video)
  * [#39) Quiz: Dictionaries](https://vt.instructure.com/courses/66476/assignments/356621)
  * [#39) Programming: Dictionaries](https://vt.instructure.com/courses/66476/assignments/356679)

###  &icon-educators; Lesson

Download Slides:
[Dictionaries.pptx](https://vt.instructure.com/courses/66476/files/6544357/download?verifier=y0FnaaNc1nPVQme8ZCTjCAaw0VSbu0SUZHfoblBU&wrap=1
"Dictionaries.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Dictionaries"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/hNlvXdv0fTQ?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Dictionaries:**  
Let's learn about Dictionaries.

**Slide 2 - Dictionaries:**  
Dictionaries are one of the most flexible and useful data structures in
programming. The idea of a dictionary is that they map from keys to values.
Think of it like an actual dictionary: given a word, you can look up its
definition. This lookup has a large number of applications.

**Slide 3 - Dictionary Literals:**  
The syntax for a dictionary literal begins with a pair of curly braces. Inside
of those braces, you will find key/value pairs separated by commas. Each key
is separated from its value with a colon. The key and the value can be any
expression, but are often literal values. Although not required, each key-
value pair is often placed on its own new line.

**Slide 4 - Keys:**  
The keys of a dictionary are what we use to look up information. The keys of a
dictionary are unique. Typically, the keys will be of the same type, although
this is not a requirement.

**Slide 5 - Keys:**  
Each key is mapped to a value. With the appropriate key, we can get a desired
value. Values do not have to be unique, unlike keys. Like keys, the values can
be of any type, even if they are not the same.

**Slide 6 - Dictionary Access:**  
The values of a dictionary can be retrieved using dictionary access. Another
similarity between lists and dictionaries is how both use square brackets.
With lists, we used numeric indexes to access elements. With dictionaries, we
use the keys. Often, the keys will be strings, so often we will see strings
inside the square brackets.

**Slide 7 - Lookups:**  
When we perform dictionary access, we give a key, and the dictionary access
expression is replaced with the corresponding value. If the key is not in the
dictionary, a " KeyError " is raised. A common mistake is to use a value
instead of a key, which will also cause a " KeyError ".

**Slide 8 - Membership Test:**  
Dictionaries, like lists or strings, are sequences. They can possess any
number of key-value pairs. You can test if a specific key is in a dictionary
using the in operator, the same way you would test for lists or strings.

**Slide 9 - Not Always Strings:**  
Sometimes keys will be strings, but it turns out that anything can be a key.
If a dictionary maps integers to strings, for instance, then the keys will be
integers. In fact, it is possible for a dictionary lookup to appear just like
a list lookup!

**Slide 10 - Sequence:**  
Dictionaries are a sequence of key/value pairs. Therefore, you can iterate
through them like a list. However, there are three different ways to iterate
through them: Through their keys, their values, or their keys and values at
the same time. Notice how thist last approach gives us the key and value at
the same time!

**Slide 11 - Terminology:**  
A final minor note about dictionaries: dictionaries are also sometimes known
as maps, tables, or hashes. Although there are subtle differences in this
terminology, the idea is still roughly the same each time.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

A dictionary maps keys to values. Looking up data in a dictionary is very fast
and convenient. Keys and values in a dictionary can be set on the fly, which
makes them an extremely powerful tool for solving many kinds of problems.