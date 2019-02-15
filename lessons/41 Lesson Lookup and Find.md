In this lesson, we will learn the difference between finding in a list and
looking up in a dictionary

###  &icon-check-plus; Objectives

  1. Replace a find operation with a lookup
  2. Explain the advantage of a lookup operation vs. a find operation

###  &icon-quiz; Activities

  * [#41) Lesson: Lookup and Find](#video)
  * [#41) Quiz: Lookup and Find](https://vt.instructure.com/courses/66476/assignments/356591)

###  &icon-educators; Lesson

Download Slides: [Lookup and
Find.pptx](https://vt.instructure.com/courses/66476/files/5919800/download?verifier=x4BKeMUHZSAqlJoJcEYTAozjtW4A9Akk3ntKS9qH&wrap=1
"Lookup and Find.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Lookup and Find"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/nyYJLLPxOAM?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Lookup and Find:**  
Let's learn about Lookups and Finding.

**Slide 2 - Lists vs. Dictionaries:**  
Both lists and dictionaries are collections of data. You can use them to store
and retrieve data later. However, which one you use can have performance
implications.

**Slide 3 - Finding in a List:**  
Say we have a list of strings that represent names. If we want to determine
whether a particular string is in the list, we must walk through each element.
If there are 10 strings, this will not take long. But what if there are many,
many strings, like in the University's directory? Finding a string in a list
will take longer when there are more elements.

**Slide 4 - Looking up in a Dictionary:**  
However, if you use a dictionary to store names (perhaps mapped to their
address or grade), then you can look up keys instantly. On average,
dictionaries' lookup does not take longer no matter how many elements there
are. This is a major advantage of dictionaries over lists.

**Slide 5 - Choosing Data Structures:**  
Lists are great when you need to go through many items in a specific order.
Dictionaries are great when you need to lookup a single item. Think carefully
about your use case, and choose an appropriate data structure.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Finding an element in a list is much slower than looking up a key via a
dictionary.