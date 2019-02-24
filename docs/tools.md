This section details the software tools leveraged in this course:

# Coding Environments

## BlockPy

BlockPy ([https://think.cs.vt.edu/blockpy/](https://think.cs.vt.edu/blockpy/)) is a web-based, dual block/text coding environment for Python that has a sophisticated autograder. This autograder can be setup to assess students' programs in a number of ways beyond just unit testing: their code can be checked for the presence or absence of structural elements, their code can be run against different inputs, and a complex flow analyzer and type inferencer can detect bad code patterns (e.g., initializing and then never using a variable).

BlockPy features a block interface, but most students do not need or want this feature. Therefore, they will typically work in the text interface. The block and text interfaces are kept in sync with each other, if students choose to use those interfaces. They are also able to write their code in an external editor and upload their code instead.

As a research project, BlockPy is an ongoing effort that has many advantages over a traditional editor, but also some key disadvantages. Not every Python feature is available (e.g., at the time of writing, you cannot write to files or import certain libraries like Pandas). Developing new problems requires some expertise with the Instructor API (although we are in the process of simplifying this). Some reasonable alternatives to BlockPy could be:

* CloudCoder (although this does not seem to have LTI support)

* CodeWorkout (although their python support is in progress)

* CodingBat (although their problem collection is limited)

## Anaconda

Installing Python is ultimately necessary in the course, but will be a bit of a headache when it comes to managing packages and versions. Therefore, we use the Anaconda distribution ([https://www.anaconda.com/download/](https://www.anaconda.com/download/)) to simplify installation. This not only install Python, but popular packages (MatPlotLib, Requests) and tools (Jupyter Notebooks and Spyder). Further, the built-in Conda package manager offers a more extended set of pre-built packages if further packages are necessary.

## Spyder

Students need experience with a real programming environment. BlockPy is great for small structured activities, but not sufficient for larger projects. Further, working in a real editor is important for students to develop real-world expertise. Therefore, we use Spyder, because it comes packaged with Anaconda.

Spyder is a professional, Data Science oriented programming environment. Besides an integrated editor and console, it also has an integrated debugger and several other useful features. It can be somewhat cumbersome, but seems to be stable enough. However, as of 2018 it is being deprecated and will not be supported. Some reasonable alternatives to Spyder could be:

* Pycharm (a professional programming environment for Python on par with Eclipse or IntelliJ IDEA)

* Thonny (described below)

* Jupyter Notebooks (described below, but not necessarily suitable for all projects)

* Wing (a fairly modern python editor)

* Idle (do not use Idle, it is a garbage editor)

## Jupyter Notebooks

Jupyter Notebooks is a professional tool for developing reports, popular in many data science and research communities. Jupyter allows you to embed code, the results of the code, and prose into one document. Afterwards, students can download an HTML representation of their document. BlockPy has support for grading Jupyter Notebooks. 

JupyterLabs is a modern evolution of Jupyter Notebooks that features a more full featured programming environment. It could be investigated as a potential programming environment, although its sensibilities are more for document writing than system development.

## NotePad++/Sublime

In the first semester, students were not required to install any programmer-friendly text editors. Therefore, their operating system did not have any applications registered to open .PY files (or other special data files). Students would use various pieces of software (e.g., Word) to open documents, and would also get alarmed when they could not "see" their Python files. Therefore, we now have them install a modern text editor that registers with their files. We do not mandate a specific editor, but have a whitelist of acceptables ones. Most students are recommended to use NotePad++ on Windows and Sublime on Mac.

## PythonTutor

The online PythonTutor website (http://pythontutor.com/visualize.html) is a powerful way to visualize code. Not only will it perform step-by-step statement-level execution, but it will also visualize memory layout. Code can be shared, and instructors can even instantiate an interactive, collaborative session. I have used PythonTutor during class demos and particularly in one-on-one tutoring sessions.

## Thonny

This is a beginner-friendly Python IDE (http://thonny.org/), and I would describe it as on-par with Spyder in terms of features. A major advantage it has over the PythonTutor is that it can step through expressions (as opposed to statements); a disadvantage is that it doesn't do the cool memory layout that PythonTutor does. During in-class demos and office hours, I have used both Thonny and the PythonTutor to highlight certain ideas. Thonny is in active development and seems to have some strong potential - I would recommend it as a potential replacement for Spyder.

* Update: The latest versions of this course use Thonny instead of Spyder

# Environment

This course follows a blended model, which means that there is both a physical aspect to the class and a digital environment. This section describes the requirements for these environments.

**Physical Environment: **The classroom has few specific requirements:

* The instructor should have some place to project slides.

* TAs and instructors should be able to physically approach and interact with individual students.

* Ideally, each student will have access to power for their laptop.

* If possible, students should have enough proximity to turn and talk to each other during the peer instruction activities.

**Digital Environment**: A modern LMS (e.g., Canvas, which is what we used) should be used to:

* Distribute video lessons

* Administer and auto-grade quizzes

* Integrate with LTI tools like BlockPy and Web-CAT

* Provide a platform for collecting and grading the larger-scale projects
