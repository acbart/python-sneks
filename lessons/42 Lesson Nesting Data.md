In this lesson, we combine the ideas of lists and dictionaries in order to
create nested data structures. With nesting, we can describe much complex
things from the real-world in data.

###  &icon-check-plus; Objectives

  1. Explain how complex types can be nested
  2. Write syntactically correct Lists and Dictionaries literal values
  3. Write syntactically correct literals that compose multiple types
  4. Write statements and expressions that access data in nested data structures
  5. Describe complex nested data in succinct forms

###  &icon-quiz; Activities

  * [#42) Lesson: Nested Structures](#video)
  * [#42) Quiz: Nested Structures](https://vt.instructure.com/courses/66476/assignments/356633)
  * [#42) Programming: Nested Structures](https://vt.instructure.com/courses/66476/assignments/356682)

###  &icon-educators; Lesson

Download Slides: [Nested
Structures.pptx](https://vt.instructure.com/courses/66476/files/5919839/download?verifier=DESlowzA1fg6RKRcmwtODEshR92dE43bI18Rkbnv&wrap=1
"Nested Structures.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Nesting Data"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/xPs1tavJ85Q?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Nesting Structures:**  
Let's learn about Nesting Structures

**Slide 2 - The Types:**  
At this point, we've learned about 7 different types. The 5 primitive types
are Integer, Float, Boolean, String, and None. The 2 composite types we've
seen so far are Lists and Dictionaries. These 2 new composite types are
special because they are composed of other types.

**Slide 3 - The Types:**  
There are actually many more composite types in Python. In fact, there are
even ways to create entirely new primitive and composite types. But for now,
we'll stick to these basic 7 types.

**Slide 4 - Types in Types:**  
With lists, we learned that composite types had subtypes. For example, you
could have a List of Integers. Dictionaries have multiple subtypes, one for
each key and one for each value. For example, you could have a dictionary that
maps String Keys to Float values.

**Slide 5 - Nesting Types:**  
You can also use composite types as subtypes. In other words, you can have
lists of dictionaries or dictionaries of lists or even lists of lists. There
are no practical limits to how many times you can nest composite types.

**Slide 6 - Nesting Literals:**  
Let us look at a concrete example. Shown here is a list of dictionaries. Each
dictionary is being used as a Record with the same keys; these dictionaries
can therefore represent a bunch of animals. The subtype of the list is
dictionary. The keys of those dictionaries are all strings, and the values are
either strings or integers.

**Slide 7 - A Representative Element:**  
To quickly understand the structure of a complex nested structure, we find it
useful to model the memory. In the diagram below, we see that we have a list
of dictionaries, where the named keys map to different types.

**Slide 8 - Processing Nested Data:**  
As you process this complex nested data's structure, you have to stay aware of
where you are. This is similar to needing to navigate a maze. Consider a list
of dictionaries like the one shown before. If we wanted to print the name of
each animal, we would first need to process them a list using a For loop.
Then, we can process an individual dictionary.

**Slide 9 - Nested Dictionaries:**  
Here we see a dictionary that is composed of dictionaries. When we access
these nested dictionaries, we use square brackets chained together. The
expressions on the right access various elements of the dictionary. Nesting
dictionaries is an excellent way to cluster information.

**Slide 10 - Layers of Nesting:**  
As previously mentioned, there are no limits to how much nesting can happen.
Here we see a list of dictionaries of dictionaries, to represent an event
calendar. Instead of processing this list with a for loop, we can chain list
indexing and dictionary access to lookup specific elements. As our nested
structures grow more complex, it becomes more and more important to understand
the nature of the data to learn to navigate it.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Lists and Dictionaries are both complex types, which means that they are
composed of other types. Not just primitive types, but even other complex
types. This means that you can have lists inside of dictionaries, and
dictionaries inside of lists. This richer representation allows us to model
much more complex stuff.