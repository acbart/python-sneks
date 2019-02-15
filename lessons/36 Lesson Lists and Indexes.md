In this lesson, we will learn the idea of processing indexes, and why this is
discouraged in Python.

###  &icon-check-plus; Objectives

  1. Iterate through a list by its indexes
  2. Explain why you should avoid iterating by indexes

###  &icon-quiz; Activities

  * [#36) Lesson: Lists and Indexes](#video)
  * [#36) Quiz: Lists and Indexes](https://vt.instructure.com/courses/66476/assignments/356635)

###  &icon-educators; Lesson

Download Slides: [Lists and
Indexes.pptx](https://vt.instructure.com/courses/66476/files/5919799/download?verifier=NbZdbvzuCrbQnYvgtKfuxzntiJZuBGPQ6inAvT7H&wrap=1
"Lists and Indexes.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Lists and Indexes"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/WL1VcFsogbU?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Lists and Indexes:**  
Let's learn about Lists and Indexes.

**Slide 2 - Lists and Indexes:**  
So far, we have iterated through a list using the for-each syntax to get each
value of the list. In many languages, indexes are used to access the values of
a list. The index of the list are the integers, starting from 0 and counting
up, that uniquely identify each element.

**Slide 3 - Value vs. Index:**  
The top code shown here is the preferred way to process a list, where we
iterate through each value. In Python, you can also iterate by using a
combination of the range and len functions, as shown below. The bottom way is
the less convenient index style.

**Slide 4 - Indexes Are Bad:**  
Using indexes to process lists is almost always a bad idea. First, we have
introduced new operations into the code: we call two functions and do an
indexing operation. Second, using indexes prevents us from thinking about the
individual values directly - consider the semantic difference between "name"
and "names[ i ]". Third, we are doing redundant work: Python should do the
work of walking through the list, not us.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Unlike other languages, Python is optimized to loop through values, not
indexes. Indexes complicate the already complicated process of loops.