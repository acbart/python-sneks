### Problem in S18: 21.1/21.1) Mystery Math/Strings

## Learning Objectives:

  * Reading and responding to unit tests
  * Explain how functions are tested for correctness 
  * Interpret a failing unit test

## Problem: The function below fails its unit test. It is supposed to consume
two numbers, do something, then return the result. Determine what the function
is supposed to do then fix it so it passes unit tests.

```html

def mystery_machine(a, b):
    return 0
print(mystery_machine(1,2))
```

### Step 0: Understanding the problem

In this case we have no idea what the function is supposed to do, so we have
to figure it out. While this may seem daunting, understanding how unit tests
work can help us out.

### Step 1: How do unit tests work?

When you click run, Blockpy does a lot more than simply run your code and
check the output for correctness. If it only checked your output, you could
pass every programming problem by simply printing the expected output instead
of doing the problem. Behind the scenes, Blockpy runs the code you wrote and
then also runs unit tests. These unit tests run the function you wrote a bunch
of times with all kinds of different inputs and compares the result to the
expected output. As soon as one of these tests fail, the unit tests stop and
gives you the “Incorrect Answer” message. If all the unit tests pass, you get
the “Correct Answer” message. We can use this knowledge to figure out what the
expected output of our mystery function is by running the unit tests.

### Step 2: Run the unit tests.

To determine the expected output, we can run the unit tests to see what the
expected output is for a given input. Here’s the result

Feedback: Incorrect Answer  
Instructor Feedback  
Your mystery_machine function did not return the right value.  
Given arguments: `2, 2`  
Expected return: `4`  
Actually returned: `0`

### Step 3: Determining the functionality:

So when we give our function the numbers 2 and 2, it should return 4. We know
2*2 is 4 so maybe our function is simply supposed to multiply the two numbers
and return the result.

### Step 4: Trying our guess

Now that we think we know what mystery_machine should do, lets run the unit
tests again. After modifying the function.

```html

def mystery_machine(a,b):
    return a * b
```

After running the unit tests again, this is our output:

Feedback: Incorrect Answer  
Instructor Feedback  
Your mystery_machine function did not return the right value.  
Given arguments: `4, 3`  
Expected return: `7`  
Actually returned: `12`

Looks like our function pass the first unit test (input of 2 and 2) but failed
the test when it was given 4 and 3. The expected output was 7 but our function
produced 12. Based on this we realize `mystery_machine` is actually supposed
to add the two numbers, not multiply them. This will pass the first unit test
because 2+2 produces the expected 4, and the second because 4+3=7.

### Step 4: Trying again:

Let’s modify the function again to return the sum of the two numbers instead
of the product and run the unit tests again.

```html

def mystery_machine(a,b): 
    return a+b
```

This time the unit test gives us this output:

Feedback: Complete  
Complete!  
Great work!

That’s it! Just based on the unit test results we were able to figure out what
the function is supposed to do. When we already have an understanding of what
a function is supposed to do and we think it should work, unit tests can help
us figure out situations where our function produces the wrong output for
certain edge cases.