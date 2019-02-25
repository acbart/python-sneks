# Module 2 - Strings and Calling Functions

More about strings, and information about string operations (e.g., indexing). Using built-in functions and methods.

### Before the week begins

N/A

### Major Topics

* How to read error messages (particularly the line number and error type)
* Making strings with escaped characters, triple quoted strings
* Using string operators like index and subscripting (i.e., square brackets)
* Calling functions and methods
* Using string methods

### Materials

* week2_day1_Strings.pptx
* week2_day2_Calling.pptx

### Due This Week:

* Module 1 quizzes and programming problems

### Graded This Week

* N/A

### Student Difficulty

* Low - TAs were engaged during class time, but not overwhelmed. Most student questions seemed to be answered quickly.

## Module 2 - Staff Meeting

Agenda:

* Resolve practical questions

    * InternalError: When you encounter a black InternalError in Python, you need to notify Dr. Bart as soon as possible.

* Reminder:

    * Grade Python Installation activity

    * First project this week

        * Any problems encountered by the TAs when trying the project?

* Submit TA Feedback Report on Friday

    * Summarizes what has gone well, what has not

    * Your chance to help us redevelop the course.

* Looking forward:

    * Debugging - Problem-solving strategies (wolf-fence, rubber ducks, scientific method)

    * Defining functions - syntax, basic idea and metaphor

    * Unit testing - How we determine if functions are correct

    * Return vs. Print - The difference between them

    * Scope - Variables defined inside a function cannot be used outside of it, and vice versa.

    * Ethics Activity 1: Prompt on Net Neutrality. Make sure you read over the assignment instructions and its guide. TAs are responsible for using the Rubric when grading, and you must never assign points without using the rubric. Make sure you are using the interface to grade, not assigning points randomly.

* TA Training: "How People Learn"

    * Learning Styles: The DEBUNKED theory that teaching students according to their preferred style ("auditory", "visual", "kinestic") will improve their learning. Multiple peer reviewed studies suggest this is not the case.

    * Cognitive Load Theory: A collection of useful, well-studied theories and effects that break down how people absorb information.

        * [Dual-Channel Theory](https://en.wikiversity.org/wiki/Cognitive_Theory_of_Multimedia_Learning) suggests that people learn better when multiple modalities are engaged (so talking as you write on the board, or having a text annotation on an image, is better than not). 

        * Every lesson has an Intrinsic load (necessary to complete the task), an Extraneous load (unrelated to the task), and Germane load (necessary for the learning). For example, a problem that has you tracing a FOR loop to process a list of prices requires:

            * Keeping the list of numbers in your head (intrinsic)

            * Knowing how to process a FOR loop (germane)

            * Ignoring the fact that these are prices (extraneous)

Your job as a TA is to manage student's extraneous load and avoid letting them be distracted. A common source of distraction is stress, which can be contagious, so keep your own stress levels down.

    * [Bloom's Taxonomy](https://cft.vanderbilt.edu/wp-content/uploads/sites/59/Blooms-Taxonomy-650x366.jpg): Knowledge can be categorized at different levels, which build on each other. Knowing where on the taxonomy a student is struggling (e.g., with remembering terminology, or applying a rule, or being creative) can help diagnose their misunderstanding.

    * MUSIC Model of Academic motivation: The drive and energy to complete academic tasks can come from 5 sources:

        * eMpowerment: agency and freedom to explore and direct their learning. As a TA, you have minimal power here, but finding opportunities to empower students is good ("Did you know you can change the color of the turtle's line?").

        * Usefulness: the sense of long-term and short-term benefit of learning the material. Connecting a lesson or the class goals with students' individual goals will help support them.

        * Success: the self-efficacy, or belief by the students that they can complete tasks. Programming is often hard, so helping students manage their struggle is important. Express confidence in their ability (when appropriate) to help students understand they can accomplish things given time and practice.

        * Caring: the belief that classmates, instructors, and TAs want them to succeed. Simply letting students know you're available and want to help them is a good thing.

    * [Gagne's Nine Events](http://s4.thingpic.com/images/j7/uS44Q1YxM1NADqN1c4tP6izj.png): An instructional model for designing a lesson. Making sure you hit all these elements can ensure learning in a more systematic way. In general, make sure that each lesson is a combination of Presentation of content, Participation by the student, and Feedback from the TA.

## Lessons

### Lesson 14- Error Messages 

Summary: When Python encounters a problem in your program, it raises an error message. This error message can be read to better understand what went wrong with your program. 

Learning Objectives:
* Explain an error message for different types of errors
* Recall the similarity in the terms "Error" and "Exception"
* Track down the offending line of an error message
* Choose an appropriate solution to the error message
* Track down the offending line of an error message in a called function of an external module

Activities:
* Lesson: Errors
* Quiz: Errors
* Programming: Errors

Misconceptions: _None listed so far_

### Lesson 15- String Operations 

Summary: You should now feel comfortable with representing a string in your computer, and then manipulating them. 

Learning Objectives:
* Define the concept of a string
* Create a string literal
* Create a triple-quoted string
* Incorporate escape characters into a string

Activities:
* Lesson: Strings
* Quiz: Strings
* Programming: Strings

Misconceptions:
* Students often think that strings with numbers are actually integers.
* Students sometimes confuse variables and strings.

### Lesson 16- String Operations 

Summary: Strings can be manipulated according to their own rules and operations, distinct from integers and booleans. 

Learning Objectives:
* Combine two strings
* Compare two strings
* Subscripting a character from a string
* Subscripting a range of characters from a string

Activities:
* Lesson: String Operations
* Quiz: String Operations
* Programming: String Operations

Misconceptions: _None listed so far_

### Lesson 17- Calling Functions 

Summary: Functions are a fundamental unit of programs, which we can use to break down tasks. Functions take in arguments and return data, just like programs. Functions are a powerful way for programmers to share code with each other, too. Some functions are known as methods, and are strongly associated with a value. 

Learning Objectives:
* Define the term Function
* Identify the necessary and optional parts of a Function call
* Explain the purpose of a Function
* Compare and contrast a function with a program
* Call a function with a return value
* Call a method with a return value
* Call a function with an argument
* Call a method with an argument
* Compare and contrast printing vs. returning from a function

Activities:
* Lesson: Calling Functions
* Quiz: Calling Functions
* Programming: Calling Functions

Misconceptions:
* They believe that print is a part of a function call
* They believe that print is a statement rather than a function itself

### Lesson 18- Calling Functions 2 

Summary: Python comes with a huge number of built-in functions and methods. Programmers learn how to use these by referring to documentation. In practice, functions are often called in combination with other functions, methods, and operations. 

Learning Objectives:
* Interpret documentation for a function
* Use a function based on its documentation
* Distinguish between Parameters and Arguments
* Nest a function call inside another function call
* Chain a method onto another method
* Combine functions, methods, and operators into a complex expression

Activities:
* Lesson: Calling Functions 2
* Quiz: Calling Functions 2
* Programming: Calling Functions 2

Misconceptions: _None listed so far_

### Project 1: Turtle Art

Summary: Students create a work of art using the built-in Turtle graphics module. Turtle graphics are an easy way to draw images in Python by moving a virtual turtle around the screen (turtle.forward, turtle.right, turtle.left, etc.). 

Learning Objectives:

* Download and modify starting code

* Submit a working .PY file

* Write a longer (>20 lines) program

* Call methods to accomplish a task

* Be creative

* Have fun

Misconceptions:

* After uploading their completed program, students redownload the file and attempt to open it. Their systems are not properly configured to open the file, and instead it runs. This prevents them from seeing the actual code. You will need to explain what code is and how they can open it in Spyder or their code editor.