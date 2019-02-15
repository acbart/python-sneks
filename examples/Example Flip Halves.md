## Problem: The expression used below splits a string into two parts and flips
them. Extract this expression into a function named `flip_halves` so we dont
have to rewrite the expression for every string. Then replaces the existing
expressions with function calls.

```html

print("ABCDEFG"[int(len("ABCDEFG")/2):] + "ABCDEFG"[:int(len("ABCDEFG")/2)])
print("testing"[int(len("testing")/2):] + "testing"[:int(len("testing")/2)])
print("python"[int(len("python")/2):] + "python"[:int(len("python")/2)])
```

### Step 0: Understanding the problem:

The goal here is to put the expression that flips the halves of a string into
a function. Doing this will reduce the amount of redundant code, which is the
whole point of functions. If we wanted to flip the halves of a string a bunch
of times (don’t worry about why we’d need to do that), we would have to copy
the expression and type in the string every time. If we put this into a
function, we could simply call the function, like `flip_halves("ABCDEFG")`,
and it would return the result. This eliminates the need to rewrite code and
to memorize or copy/paste the expression.

### Step 1: Understanding the expression:

The expression we need to use in `flip_halves` is the
`"ABCDEFG"[int(len("ABCDEFG")/2):] + "ABCDEFG"[:int(len("ABCDEFG")/2)]` part
of the first line, where we need to put our string wherever we see “ABCDEFG”.
The first part of the expression, `"ABCDEFG"[int(len("ABCDEFG")/2):]` gets the
last half of the string using indexing. The indexing
`[int(len("ABCDEFG")/2):]` begins at `int(len("ABCDEFG")/2)` which finds the
length of the string, divides it by 2 to find the middle, and converts that
value to an integer using `int()` because string indexes must be integers. The
end of the indexing (after the colon) is left blank to tell python to go to
the end of the string. The second part of the expression
`"ABCDEFG"[:int(len("ABCDEFG")/2)]` gets the first half in a similar way,
starting at the beginning by putting nothing before the colon and going until
the middle. The `+` in between these two parts combines the strings generated
by the indexing back into one string.

### Step 2: Creating the function:

Like in a prior example, [Make
Address](https://vt.instructure.com/courses/66476/pages/example-make-address
"Make Address" ), we start by creating the function header. Our function needs
to be called `flip_halves` and it needs to take a single string, which we can
just call string.

```html

def flip_halves(string):
```

### Step 3: Adding the expression:

Since our function needs to perform the expression above on our parameter,
`string`, we need to replace “ABCDEFG” with `string`:

```html

string[int(len(string)/2):] + string[:int(len(string)/2)]
```

Notice the quotation marks were removed. This is because instead of working
with a string literal, `"ABCDEFG"`, we are working with the variable `string`.

Now that we have changed the expression to work with the variable string, we
need to return the result. This is simply done with the return statement.

```html

return string[int(len(string)/2):] + string[:int(len(string)/2)]
```

Once our function hits this return statement, it will end and return the value
from the expression to whatever part of the code called our function. Now, our
completed `flip_halves` function is:

```html

def flip_halves(string):
    return string[int(len(string)/2):] + string[:int(len(string)/2)]
```

### Step 4: Using our function:

Now that we have a function that will flip the halves of any string we give
it, we need to modify the lines given to us to use our function instead of
using the expression directly. This is simply done by calling our function,
passing it the proper string:

```html

flip_halves("ABCDEFG")
```

We also need to print the return value:

```html

print(flip_halves("ABCDEFG"))
```

Doing this for every line that we had originally we get:

```html

print(flip_halves("ABCDEFG"))
print(flip_halves("testing"))
print(flip_halves("python"))
```

### Solution:

Now we can put it all together, making sure our function is before the lines
we call it so python knows it exists:

```html

def flip_halves(string):
    return string[int(len(string)/2):] + string[:int(len(string)/2)]

print(flip_halves("ABCDEFG"))
print(flip_halves("testing"))
print(flip_halves("python"))
```

As you can see, writing functions for often repeated parts of code makes
things a lot less tedious by removing the need to copy and paste, less error
prone for the same reason, and makes it easier to read and understand.