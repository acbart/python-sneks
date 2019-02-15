In this lesson, you will learn about using Files in Python. Files are an
important part of making programs useful, because they allow us to persist
information between runs of a program. Commonly, we obtain many different data
files, and write a single program that can operate across many files of the
same type.

###  &icon-check-plus; Objectives

  1. Define the term File
  2. Explain the difference between a File and a String
  3. Properly open and close a file using the With block
  4. Differentiate between a File, it's name, it's path, and it's handle
  5. Read an entire file into memory
  6. Read a file using line by line iteration

###  &icon-quiz; Activities

  * [#45) Lesson: Files](#video)
  * [#45) Quiz: Files](https://vt.instructure.com/courses/66476/assignments/356628)
  * [#45) Programming: Files](https://vt.instructure.com/courses/66476/assignments/356684)

###  &icon-educators; Lesson

Download Slides:
[Files.pptx](https://vt.instructure.com/courses/66476/files/5919824/download?verifier=kJjUaxlgn0rLqQbr7EvZX6UlkdrOvsTixV16Y9OG&wrap=1
"Files.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Files"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/FDwlMk7cFFE?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Files:**  
Let's learn about Files

**Slide 2 - Files:**  
You can think of a File as a string of data. If we know the path and filename
of the File, we can use Python to get access to it.

**Slide 3 - Opening:**  
Before you can access a file, you must explicitly open the file using the
"open" function. This function consumes the path to the file as a string and
returns a file object. Typically, we store this file object into a variable.

**Slide 4 - Reading:**  
The primary way to get data from a file is to use the ".read()" method. This
simply returns the contents of the file as a single string. Check out this
example, where we open the file, read the file handle, and then print the
text. Notice how this is a multi-step process: we use the path to open the
file, and then we read from that open file.

**Slide 5 - For Loops and Files:**  
Often, we want to process a file line-by-line. Because a File is actually a
sequence of strings (each separated by a new line), we can process it using a
For loop quite easily. The example shown will process the file line-by-line,
which would be perfect if we wanted to manipulate each line of the file,
perhaps to adjust capitalization or convert it to a number.

**Slide 6 - Closing Files:**  
When you are done with a file, you should always remember to close it using
the "close" method. It's like leaving a house: if you open a door, you need to
close the door.

**Slide 7 - FileNotFoundError:**  
Filesystems are tricky, because everyone has a different setup. Often, we
misplace files. When we try to open a file that does not exist, Python raises
an FileNotFoundError and will suggest the file does not exist. Typically, you
should check that you know the exact filename, that you are using the path,
and that you know where your Python source file is relative to the file you
are opening.

**Slide 8 - Example File Processing:**  
Processing books is one possible application for files, but often we want to
process a file full of numeric data. Here, we see some example code that will
process a list of numbers in a file, each of which represents a score. We are
also using the Sum pattern we learned about before to add each of those scores
together. Notice how we must strip off the new lines at the end of each line,
and then convert that line to a number; when we read data from a file, it
comes in as a string.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Once opened, data can be read from files in the program.