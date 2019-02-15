In this lesson, you will learn how to use the json module to access files
stored in the JSON format.

###  &icon-check-plus; Objectives

  1. Define the term "File Format"
  2. Compare and contrast the JSON format with a basic text format
  3. Use a named parameter to call a function

###  &icon-quiz; Activities

  * [#47) Lesson: File Formats](#video)
  * [#47) Quiz: File Formats](https://vt.instructure.com/courses/66476/assignments/356644)
  * [#47) Programming: File Formats](https://vt.instructure.com/courses/66476/assignments/356686)

###  &icon-educators; Lesson

Download Slides: [File
Formats.pptx](https://vt.instructure.com/courses/66476/files/5919823/download?verifier=WE4HP1g9KfIQUnTCAOKBicvDjp5pmEYc7xb59BXG&wrap=1
"File Formats.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="File Formats"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/KVkxhbXGks0?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - File :**  
Let's learn about File Formats.

**Slide 2 - File Formats:**  
When data is placed into a file, it often follows a regular structure. That
way, other users of the file can navigate the data more easily. This structure
is known as a file format. Typically, a file's format is used to determine
it's extension. This is why Python files have a ". py " at the end - even
though they are text, they are structured according to the Python language.

**Slide 3 - Recall: Opening a File:**  
Usually, regardless of the file format, we begin using it by opening the file.
Recall how we open text files using the open function, giving us a file
object. Previously, we then read the file directly. Instead, we will now use
special modules to read a file.

**Slide 4 - JSON Format:**  
The JSON format is a particularly useful format, and is available in many
programming languages. The JSON format lets you store lists, dictionaries, and
simple primitive types in a file. When you load the data, you get the same
structure back. The example shown demonstrates how easy this is. The "data"
variable could now hold a complex nested structure of data, without having to
embed it in the program.

**Slide 5 - Quickly Visualizing Data:**  
Have a complex data structure, like a list of dictionaries? Here's a quick
pattern for easily visualizing the first element. A very curious thing to note
is second parameter for this function call. This is known as a "keyword
argument", and we have to explicitly give both the parameter and the argument.
The syntax is similar to an assignment, except all of it is embedded in the
function call.

**Slide 6 - CSV Format:**  
Comma-Separated Values, or CSV, files are another very popular way to share
data. An advantage of CSV files is that they can be opened in programs like
Excel, edited like text files, or processed in programming languages like
Python. To process a CSV File, you need to use the csv reader function, which
can be a little complex. This is a situation where referring to documentation
and using Google is necessary.

**Slide 7 - Other Formats:**  
There are many, many other file formats out there. Some text formats are easy
to process, but others require special libraries. When encountering a new
format, you should always check to see if there is a module available to load
the data.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Files are often organized according to a particular format, which can make it
much easier to access the data inside.