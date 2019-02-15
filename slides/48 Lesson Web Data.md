In this lesson, you will learn how to access data from the internet directly
in Python. Although you could download web data as a file, it is often very
convenient to download the data programatically. You will learn how to do so
very easily using a module named "Requests".

###  &icon-check-plus; Objectives

  1. Retrieve structured data from a URL algorithmically using Requests
  2. Retrieve data from a web page algorithmically using Requests
  3. Extract data from an HTML page using BeautifulSoup
  4. Extract data from a string using Regexes
  5. Identify practical applications of downloading data from the internet
  6. List hazards of using data through the web.

###  &icon-quiz; Activities

  * [#48) Lesson: Web Data](#video)
  * [#48) Quiz: Web Data](https://vt.instructure.com/courses/66476/assignments/356611)
  * [#48) Programming: Web Data](https://vt.instructure.com/courses/66476/assignments/356687)

###  &icon-educators; Lesson

Download Slides: [Web
Data.pptx](https://vt.instructure.com/courses/66476/files/5919809/download?verifier=CRgZLGwVievBhYsMEz8yBYkxnyCYybUOvif073K5&wrap=1
"Web Data.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Web Data"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/UPzOMrhzK5s?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Web Data:**  
Let's learn about Web Data.

**Slide 2 - The Internet is Great:**  
One of the reasons the internet is great is that it makes it easy to share
data. This data can be access programmatically and processed in a program.
Most modern programming languages, like Python, make it easy to access web-
based data.

**Slide 3 - Internet as a Dictionary:**  
The internet can be seen as a giant Dictionary being used as a Record. You
access URLs (which are strings) and get back web pages (which are also
strings). This simplifies a tremendous number of very complex pieces of
hardware and software, but this is the result at the end of the day. Look up a
URL, get some string data back. We'll use a library that makes it just this
easy in Python.

**Slide 4 - Requests:**  
There are many ways to retrieve data from the internet. The Requests library
is one such tool. This library is not part of the standard library, but comes
with Anaconda. To get started with the Requests module, we begin by importing
it.

**Slide 5 - A Basic Request:**  
The Requests module has a number of useful functions, but in this lesson we
only need one: get. The get function consumes a URL as a string, and returns a
Response object. This response object can be a confusing thing at first, but
it is actually very easy to use.

**Slide 6 - Text:**  
To get the webpage as a string of data, you can use the "text" attribute of
the Response object. Keep in mind that most websites are written in a language
called HTML, which can be tricky to parse. So for now, we'll access simple
text websites.

**Slide 7 - JSON:**  
If the text content we retrieve from the website happens to be in the JSON
format, Requests has a simple way to process it using the JSON method.
Confusingly, JSON is a method call instead of an attribute, so make sure you
DO use parentheses with it (unlike the "text" attribute). Here, we use a
website that returns the current date and time as a JSON object.

**Slide 8 - The Internet is Hard:**  
Connecting to the internet can be problematic. Websites go down, URLs change,
your internet can get disconnected, and many other issues are possible.
Usually, you should avoid repeatedly accessing web data if you can help it.
Instead, you should download a file directly and use that. Still, accessing
websites programmatically is a frequent tool in many real-world problems.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Requests is the name of a powerful module for quickly and easily retrieving
data from the internet. Accessing web-based data is one of Python's great
strengths and has many practical applications in real life.