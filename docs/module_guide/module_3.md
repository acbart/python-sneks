# Module 4 - Using Functions

Creating simple functions.

### Before the week begins

### Major Topics

* Stategies for debugging programs

* Basic syntax and idea of creating functions. 

* Reading and responding to unit tests

* The difference between printing and returning

* Interpreting function scope

### Materials

* week3_day1_Functions.pptx

* week3_day2_MoreFunctions.pptx


### Due This Week:

* Module 2 quizzes and programming problems

* Project 1

### Graded This Week

* Python Installation Activity

### Student Difficulty

???

## Module 3 - Staff Meeting

Note: Most TA training materials come directly from:

    Luther A. Tychonievich (2017) Training Course for Teaching Assistants in Computing, <https://www.cs.virginia.edu/luther/ta-training>. Accessed 2019-02-25

* Reminders:

    * Python Installation activity must be graded this week

    * First project is due this week (Turtle graphics)

        * Grading is binary and simple - they either completed the instructions or did not. Common issues:

            * Did not draw a black border? No points.

            * Uploaded code as a screenshot? No points.

            * Uploaded code in a word doc? No points.

            * Drew a single line and gave up? No points.

    * TA Feedback Report was due on Friday

* Ethics Activity

    * Read the assignment description

    * Read the guide

    * Prompt: Net Neutrality

    * Demonstration of grading assignment through Canvas.

        * ASSIGN POINTS THROUGH THE RUBRIC, NOT AT RANDOM

* Project 2: Magical Banking

    * Context: writing an app to approve or reject loans for a magical bank

    * Need to integrate weird code from a grumpy co-worker, without touching it.

    * Main goal is to learn about program flow and satisfying unit tests

    * Write a function that calls several other functions, and also define those functions

    * Each function is individually very simple, but the combination of all of them will be challenging for some students who have not incorporated these ideas.

    * Difficulty level is higher than last project, hopefully around a 2-4 hour project for most students.

    * Expect many students to ignore the unit tests

    * Added problem: students will be using web-cat for the first time.

    * You'll need to try it out and complete it yourselves

    * Monday Class:

        * Room organized into color groups using construction paper

        * Start with brief lecture highlighting project components

        * Students are encouraged to work together on handout assignment (function tables) and the first two functions (print_introduction and input_name)

        * Also have a reference sheet with info about reading output diffs

        * Your role: mark down who completed the assignment (you'll have a spreadsheet of names), make sure they have completed it correctly -> simpler if they work together and you can grade multiple at the same time.

        * Answer questions, but try to answer groups instead of individuals - steer people towards their peers

        * Each TA will have their own color that they're responsible for (about 20-30 students each). One TA will be a Meta TA walking around helping out as needed

        * Goal: get them started on the project, via fostering community

* Looking forward:

    * Documenting - Writing comments and multi-line comments

    * Function Development - creating more complex functions, particularly by extracting repeated code

    * Data Flow - seeing how values flow through a program

* TA Training: Problem Students I

    * "You are a Teaching assistant, not a Passing assistant".

    * 3.1 Students who want the answer, not learning

        * Ask questions

        * Solve in a different context

        * Make them do something before going on

        * Look at them, not the computer

        * Say "no"

        * Avoid becoming an oracle

        * https://www.cs.virginia.edu/luther/ta-training/students.html#students-who-want-the-answer-not-learning

    * 3.2 Students whose question is answered in the assignment writeup

        * Ask them "Please go to the assignment writeup. Read it aloud to me."

        * https://www.cs.virginia.edu/luther/ta-training/students.html#students-whose-question-is-answered-in-the-assignment-writeup

    * 3.3 Students who insist on doing it the wrong way

        * Neither force nor ignore

        * Give them a choice, "I can provide excellent help with a better approach, or vague help with your current approach."

        * https://www.cs.virginia.edu/luther/ta-training/students.html#students-who-insist-on-doing-it-the-wrong-way

    * 3.5 Students who seem not to have attended class or read the textbook

        * If you have tons of time, you can teach them

        * But otherwise, redirect them to the course resources (book, slides, google)

        * If they refuse, then you can refuse to help them.

        * https://www.cs.virginia.edu/luther/ta-training/students.html#students-who-seem-not-to-have-attended-class-or-read-the-textbook


## Lessons

### Lesson 19- Debugging Techniques 

Summary: When you encounter an error, you should attempt to debug them (using print statements, meticulously explaining your code, etc.). 

Learning Objectives:
* Choose the most suitable debugging method to debug a program
* Compare and contrast different debugging techniques
* Explain how you can use automatic tracing tools to debug a program
* Explain how you can use print debugging to debug a program
* Explain how you can use code tracing to debug a program
* Explain how you can google to debug a program
* Explain how you can use rubber duck debugging

Activities:
* Lesson: Debugging
* Quiz: Debugging

Misconceptions: _None listed so far_

### Lesson 20- Defining Functions 

Summary: Function definitions have a body of code and are described by their header. Creating functions is necessary for building up programs of scale. 

Learning Objectives:
* Determine if a situation could benefit from a function
* Break down a complex task into multiple function calls
* Identify the scope of variables in and outside of a function
* Define a function with a return value
* Describe the difference between parameters and arguments
* Define a function without parameters
* Define a function with parameters
* Extract a variable from a function into a parameter
* Describe the signature of a function

Activities:
* Lesson: Defining Functions
* Quiz: Defining Functions
* Programming: Defining Functions

Misconceptions:
* Students believe that any code should be encapsulated in a function, instead of code that needs to be reused or worked on in isolation.
* Students attempt to add "types" to the arguments by surrounding the parameter names with quotes, square brackets, and other literal symbols.
* Students attempt to nest function definitions into other control structures
* Students print instead of using return

### Lesson 21- Unit Tests 

Summary: Unit tests are used to ensure that a function is correct. 

Learning Objectives:
* Explain how functions are tested for correctness.
* List advantages of using unit tests
* Intepret a failing unit test
* Describe the limitations of unit tests

Activities:
* Lesson: Unit Tests
* Quiz: Unit Tests

Misconceptions: _None listed so far_

### Lesson 22- Return and Print 

Summary: Returning from a function causes a value to be made available at the callsite. Printing from a function makes a value appear on the console. 

Learning Objectives:
* Differentiate between a return statement and a print function
* Identify the output of a function that does not return anything
* Identify the output of a function that prints instead of returns
* Identify a callsite

Activities:
* Lesson: Return and Print
* Quiz: Return and Print

Misconceptions: _None listed so far_

### Lesson 23- Scope 

Summary: Variables created inside a function cannot be used outside the function, and variables created outside a function should not be used within. 

Learning Objectives:
* Determine whether a variable is available within a function.
* Determine whether a variable is available outside a function.
* Determine whether a variable is aliased within a function.
* Define the difference between a global variable and a local variable.
* Explain why global variables are bad.

Activities:
* Lesson: Scope
* Quiz: Scope

Misconceptions: _None listed so far_

### Lesson 24- Documenting 

Summary: Documentation is a helpful tool for the benefit of programmers to better organize code. There are several ways to document in Python, but typically functions are documented using multi-line comments that describe the function's inputs, outputs, and purpose. 

Learning Objectives:
* Create a single-line comment
* Create a multi-line comment
* Differentiate between a single- and multi- line comment
* Explain the limitation of multi-line comments
* Explain the purpose of documentation
* Document a function's inputs, outputs, and purpose

Activities:
* Lesson: Documenting
* Quiz: Documenting

Misconceptions: _None listed so far_

### Lesson 25- Function Development 

Summary: Functions allow us to extract commonly repeated chunks of code. 

Learning Objectives:
* Use functions to solve problems
* Evaluate the name of a function
* Extract code into a function
* Define functional decomposition

Activities:
* Lesson: Function Development
* Quiz: Function Development
* Programming: Function Development

Misconceptions: _None listed so far_

### Lesson 26- Data Flow 

Summary: Data enters a function through parameters and leaves through returns. To make data available between functions, it will need to be returned. 

Learning Objectives:
* Describe how data flows between two chained functions.
* Explain how values defined in one function can flow to another function.
* Describe how user input introduces new values

Activities:
* Lesson: Data Flow
* Quiz: Data Flow

Misconceptions: _None listed so far_

