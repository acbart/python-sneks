In this lesson, you will learn how you can organize code into modules. Modules
are a collection of code, and particularly functions. Rather than sharing
functions directly, programmers actually share modules. You will learn how to
use other modules to access more functions.

###  &icon-check-plus; Objectives

  1. Define the term "Module"
  2. Write code that imports a module
  3. Write code that uses functions defined in an external module
  4. Create a module

###  &icon-quiz; Activities

  * [#46) Lesson: Modules](#video)
  * [#46) Quiz: Modules](https://vt.instructure.com/courses/66476/assignments/356639)
  * [#46) Programming: Modules](https://vt.instructure.com/courses/66476/assignments/356685)

###  &icon-educators; Lesson

Download Slides:
[Modules.pptx](https://vt.instructure.com/courses/66476/files/5919838/download?verifier=dRQhIFfd8rSgaEJkBsGh5Deeh0QYKkDc86RgCZFn&wrap=1
"Modules.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Modules"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/nDnEA0T_aSU?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Modules:**  
Let's learn about Modules.

**Slide 2 - Modules:**  
Whenever you create a new Python program, you are actually creating a Module.
In other words, a module is just a Python program. A module is useful,
however, because it can be imported into another module. Any functions,
variables, and other definitions created in the module will then be available
in the other module.

**Slide 3 - Terminology:**  
Modules are sometimes also known as packages or libraries. Typically, a
package is a collection of one or more modules. However, the words are all
more-or-less interchangeable.

**Slide 4 - Import:**  
To import data from another module, you use the Import statement. There are
three different ways to import a module. The simplest is shown here, where we
write the keyword import and the name of the module. Once a module is
imported, you can reference its definitions using the name of the module, a
period, and then the name of the function, variable, or other definition you
want to use.

**Slide 5 - Specific Import:**  
It can be bothersome to repeat the module name each time you want to use a
function. Therefore, Python has a convenient syntax for importing the
functions directly. This version uses the "from" keyword, followed by the
module name, the "import" keyword, and then the name of the function or other
definition you want to use. Afterwards, you can use the definition as if it
were defined in that file.

**Slide 6 - Longer Imports:**  
Complex packages are often divided into multiple folders containing the
modules. When importing specific parts of these packages, you will need to use
periods to indicate folder names. The result of this import is then aliased
(or renamed) using the "as" keyword. Usually, the documentation will tell you
exactly what to import; otherwise it can be difficult to infer the path. For
example, many tutorials for the MatPlotLib library (which we will learn later)
suggest you import the PyPlot module as shown here. After this import, the "
plt " module is now available.

**Slide 7 - Standard Library:**  
Python has a number of useful built-in modules called the Standard Library.
Further, Python programmers have created many other "third party libraries"
that are easy to install. Many of these modules come prepackaged in
distributions like Anaconda. We will not cover all these modules in this
course, but you will often come across them when solving real-world problems.

**Slide 8 - Installing New Libraries:**  
Although you may not have to do it very often, it is very easy to install new
modules from a command line. Simply use the "pip" command to install a module.
You will need to know the exact module name. Make sure that you have the right
module name; when you install a new module, you are trusting the developer to
not install anything malicious!

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Modules are a collection of functions and code that are shareable with other
coders. Every time you create a Python program, you are actually creating a
module. There are many modules out there.