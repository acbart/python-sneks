## Problem: Create a function called `weekend_plan` that takes 2 parameters.
The first parameter should be a boolean that is true if you have homework due
on Monday and false otherwise, and an integer the represents your age. The
function should capture the following logic

```html

If you have homework due,
    print "Do your homework!"
If you don't have homework due and you are over 21,
    print "Tots happy hour!"
If you don't have homework, but you are under 21,
    print "Play video games!"
```

You should call your function twice to test it: once by passing literal values
and once by passing variables.

## Step 0: Understanding the problem:

We need to create a function that takes two parameters, a boolean and an
integer, and uses those values to determine and print what we should do this
weekend. This can be done using an if statement.

## Step 1: Creating the function header:

We need to create a function named `weekend_plan` that takes two parameters, a
boolean that is true if you have homework and an integer representing your
age. Since this function will be tested directly by unit tests, we need to
make sure the order of the parameters is exactly as stated in the problem.
Even though the functions have different types, Python will give values to
parameters in the order they are given. If one call to your function expects
the parameters to be in a different order than they are, you can have strange,
sometimes hard to find bugs in your code. (For example, notice if you type
`print(True &gt; 42) in python there is no error). With that in mind, our
function header looks like:

```html

`def weekend_plan(has_homework, age):
```

## Step 2: Creating the if statement:

Now that we have our function header and the parameters `has_homwork` and
`age`, we can create an if statement that captures the logic above. There are
a lot of ways to construct this if statement that would work, but we want to
find the way that requires writing the least amount of code. Notice that the
second to results (Tots happy hour and Play video games) both need
has_homework from the first part to be false. So if we put them into an else
if, abbreviated `elif`, after checking `has_homework`, we only need to check
it twice.

```html

if has_homework:
    print("Do your homework!")
elif ???   # Else if for tots    
elif ???   # Else if for video games
```

Now we know the first else if will only be checked if `has_homework` is false,
so we can simply check if you are at least 21 using the `>=` operator.

```html

if has_homework:
    print("Do your homework!")
elif age >= 21:
    print("Tots happy hour!)
elif ???   # Else if for video games
```

The final part of the if statement will only be checked if the first two
failed, meaning `has_homework` and `age >= 21` are both false. Since that is
the exact condition we need to print “Play video games”, we don’t need to
check anything at all. Code under the `else` keyword only execute if
everything else in the if statement was false.

```html

if has_homework:
    print("Do your homework!")
elif age >= 21:
    print("Tots happy hour!)
else:
    print("Play video games!)
```

## Step 2.5: Alternative if statements:

As we noted before, there are many other ways we could’ve written our if
statement that are “logically equivalent” to the statement we made. As long as
two if statement (or series of if statements) capture the same logic and
always produces the same output when given the same input, it is logically
equivalent. For example, instead of trying to write as little code as
possible, we could’ve tried to match the syntax of the logic we were given as
close as possible.

```html

if has_homework: 
    print("Do your homework!")
if not has_homework and age > 21:
    print("Tots happy hour!")
if not has_homework and age < 21: 
    print("Play video games!")
```

Notice we had to use the `not` and `and` keywords. The `not` keyword goes
before any boolean value and it gives the opposite value. So `not True` gives
False and `not False` gives True.

The `and` keyword goes between any two boolean values. As you probably
guessed, `and` is used to see if value1 AND value2 are true. If either value
is false, the whole statement is false.

Implementing the given logic using multiple if statements like above makes the
code look more like the structure we were given and makes it somewhat easier
to understand when reading over it. However, there is a lot of redundant value
checking which is usually best to avoid.

## Step 3: Putting the function together:

Since our function isn’t meant to return anything, all we need to do is put
our if statement in the function

```html

`def weekend_plan(has_homework, age): 
    if has_homework: 
        print("Do your homework!")
    if not has_homework and age > 21:
        print("Tots happy hour!")
    if not has_homework and age < 21: 
        print("Play video games!")
```

## Step 4: Call our function:

When you call a function with more than one arguments, you need to make sure
you get the type and order of the arguments correct. The function we wrote
takes the `has_homework` boolean, then the `age` integer. The problem also
said we should call it once with literal values and once with variables. If
you don’t remember, a literal value is pretty much what it says: literally a
value, while a variable is something we can store values in. Some examples of
literal values are `"A string"`, `4`, `True`. So to call a function with
literal values we can just pass the values we want to use directly into the
function call:

```html

weekend_plan(True, 22)
```

For our second function call, we need to store the values we want to use in
variables first, then give the function those variables.

```html

homework_due = False
myAge = 19
weekend_plan(homework_due, myAge)
```

## Solution:

```html

`def weekend_plan(has_homework, age): 
    if has_homework: 
        print("Do your homework!")
    if not has_homework and age > 21:
        print("Tots happy hour!")
    if not has_homework and age < 21: 
        print("Play video games!")

weekend_plan(True, 22)

homework_due = False
myAge = 19
weekend_plan(homework_due, myAge)
```