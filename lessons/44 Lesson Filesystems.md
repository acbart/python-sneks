In this lesson, you will learn about your computer's File System. Files are an
important part of making programs useful, because they allow us to persist
information between runs of a program. Files are organized into directories
within your file system, and are uniquely identified by paths.

###  &icon-check-plus; Objectives

  1. Navigate a file system using the command line
  2. Identify the path of a file

###  &icon-quiz; Activities

  * [#44) Lesson: Filesystem](#video)
  * [#44) Quiz: Filesystem](https://vt.instructure.com/courses/66476/assignments/356599)

###  &icon-educators; Lesson

Download Slides:
[Filesystem.pptx](https://vt.instructure.com/courses/66476/files/5919825/download?verifier=fMg4W6JTBbkA0EOF4z0TVjeNveqSqsHxXeGU3M0o&wrap=1
"Filesystem.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Filesystems"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/_B6AeWykxfs?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Filesystems:**  
Let's learn about Filesystems

**Slide 2 - Files:**  
Your computer is equipped with a filesystem that lets you save and load files.
A file is simply a sequence of data, not unlike a string. You create files all
the time - text documents, pictures, music, python files, and so on. These
files are organized by your File System.

**Slide 3 - Directories:**  
Directories, also known as folders, are a way to group files and other
directories together. Because we can put directories inside of directories, we
end up with a heirarchical system.

**Slide 4 - Paths:**  
Think of files as a house. Directories are neighborhoods, cities, states, and
successively bigger ways to group houses. Each file has a unique address
within your file system called its "path". We use these paths to navigate
files and directories, just like we would houses and neighborhoods.

**Slide 5 - Absolute Path:**  
The full address for a file is known as its "absolute path". The exact format
of the path will depend on your platform, but typically they are a series of
folder names separated by slashes. In Python, it is typically best to use
forward slashes, since these tend to work regardless of the platform.

**Slide 6 - The Working Directory:**  
Command lines that interact with file systems have a Current Working
Directory. It's essentially "where you are" at the moment. In IPython , you
can check your current directory using the " pwd " command. PWD stands for
Print Working Directory.

**Slide 7 - Relative Paths:**  
If there are folders in your current working directory, you can reference them
without writing the Absolute path. Instead, the folder's path is simply it's
name. You can see a list of the folders in your current directory by using the
"ls" command. LS stands for "list", as in "list the files".

**Slide 8 - Moving between directories:**  
To move from one directory to another, we use the "cd" command. You can move
to an absolute path or a relative path. You can also move up a folder level by
using a pair of periods.

**Slide 9 - Commands:**  
It can be tricky to remember these commands, but knowing how to use them will
serve you well when you start working on larger projects.

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

Your computer has a File System that allows you to navigate, open, and edit
files. These files are organized so that programs can open them using their
address.