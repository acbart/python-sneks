## Problem: Write a function called `hide_password` that takes a password as a
string and returns a “hidden” password string. The hidden password string
should be the same length as the string give, but with all the characters
replaced with a question mark.

For example, the function would convert `"password"` to `"????????"`.

Call the function twice to test it (don’t use your real password, that’s a bad
idea)

## Step 0: Understanding the problem:

We need to write a function that takes a string and returns a string that is
the same length but consists of only question marks. The first thing we’ll
need to do is figure out the length of the password string then we’ll have to
create a string of question marks the same length.

## Step 1: Creating the function header:

We need to create a function called `hide_password` that takes a password
string.

```html

def hide_password(password):
```

## Step 2: Finding the length of the password:

To find the length of a string we can use the built in `len` function on the
string. This function takes in a string and returns the length of that string.
We can save that number in a variable called length

```html

length = len(password)
```

## Step 3: Creating a string of all question marks:

Now that we know how long to make the string of question marks, we need a way
to create it. Luckily python makes this easy for us by allowing us to
“multiply” strings by integers to duplicate them. For example, `"VT" * 3`
gives us the string `"VTVTVT"`. With this we can create our string of question
marks by multiplying a string with just a question mark by the length of the
password, like this:

```html

"?" * length
```

## Step 4: Return the hidden password:

We can tell our function to return the string we created in Step 3 by adding
the return statement before it:

```html

return "?" * length
```

Now all the parts of our function can be put together:

```html

def hide_password(password): 
    length = len(password)
    return "?" * length
```

## Step 5: Calling the function:

Now we need to call our function and print the result twice.

```html

print(hide_password("Password123"))
print(hide_password("12345"))
```

Side note, if either of these is your password, you should definitely change
it.

## Solution:

Putting everything together gives us the solution:

```html

def hide_password(password): 
    length = len(password)
    return "?" * length

print(hide_password("Password123"))
print(hide_password("12345"))
```