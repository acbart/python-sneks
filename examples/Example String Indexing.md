## Learning Objectives:

  * Subscript strings
  * Combine strings and/or string literals

###

## Problem: Given strings assigment_1 and assignment_2, shown below, use
string indexing to extract the due dates of each assignment and print the due
dates, separated by a comma and a space.

```python

assignment_1 = "Maze Game,Jan. 26,10pts"
assignment_2 = "Types,Feb. 2,10pts"

```

### Step 0: Understanding the problem.

The idea of this problem is that you are given two strings, assignment_1 and
assignment_2, each representing some details about a particular assignment.
The goal is to use string indexing to extract the due date from each
assignment string and print the due dates as a neatly formatted list. So the
expected output is

```python

Jan. 26, Feb. 2

```

### Step 1: Find the indexes of each due date.

0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 | 14 | 15 | 16 | 17
| 18 | 19 | 20 | 21 | 22  
---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---  
M | a | z | e |  | G | a | m | e | , | J | a | n | . |  | 2 | 6 | , | 1 | 0 |
p | t | s  
  
We can see that the due date for assignment_1 (Jan. 26) starts at index 10 and
ends at index 16. Therefore to include the entire date with string indexing we
need to put

```python

assignment_1[10:17]

```

because python stops at the character before the index given by the second
number.

Doing the same thing for assignment_2 we can see we need to use

```python

assignment_2[6:11]

```

0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 | 14 | 15 | 16 | 17  
---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---  
T | y | p | e | s | , | F | e | b | . |  | 2 | , | 1 | 0 | p | t | s  
  
### Step 2: Create the formatted (with a comma and space) due date string.

We know we can use the + operator to concatenate (combine) strings. So

```python

assignment_1[10:17] + assignment_2[6:11]

```

gives us

```python

Jan. 26Feb. 2

```

But this isn't exactly what we want. We can also concatenate string literals
using the + operator. String literals are any string values in quotation
marks. So `assignment_1` is a variable, while `"Maze Game,Jan. 26,10pts"` is
the string literal value we store in the variable. So with that in mind, we
can use

```python

assignment_1[10:17] + ", " + assignment_2[6:11] #Notice the space!

```

which gives us

```python

Jan. 26, Feb. 2

```

### Step 3: Print out the result.

To display the string created in Step 2, we can store it in a variable like
this:

```python

due_dates = assignment_1[10:17] + ", " + assignment_2[6:11]

```

then print out the variable we created:

```python

print(due_dates)

```

or, we can simply print the statement from Step 2 directly by putting it in
the print statement.

```python

print(assignment_1[10:17] + ", " + assignment_2[6:11])

```

### Solution:

```python

print(assignment_1[10:17] + ", " + assignment_2[6:11])

```