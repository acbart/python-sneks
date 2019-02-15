## Problem: You want to be able to go to a website by simply typing the name
of the website instead of the full address (e.g. typing Google instead of
https://google.com). Create a function called make_address that takes the name
of a website returns the website name with “https://” added to the beginning
and “.com” added to the end. Call this function with your 2 favorite websites
and print the results to test it.

### Step 0: Understanding the problem:

The goal here is to create a function that takes one string (the name of the
website) and returns that string with something added to  
the beginning and the end. Then we have to test the function with a few of our
favorite websites.

### Step 1: Create the function make_address:

First thing we need to do is create a function that takes a single string. We
do this using the `def` keyword (short for **define** function). A function
definition has 4 parts: the **def** keyword, the name of the function, the
names of the parameters the function takes, and a colon (‘:’). The **def**
keyword goes first, followed by function name, then the parameter names in
parenthesis, like below.

```html

def function_name(parameter1, parameter2):
```

In this case, the function name is make_address and it takes one parameter,
we’ll call it “name”. So our function definition is:

```html

def make_address(name):
```

### Step 2: Creating the web address.

To combine two strings, we can use the `+` operator. So to build our website
address we have to ‘add’ the string “https://” to the beginning of our
parameter name and add ‘.com’ to the end.

```html

"https://" + name + ".com"
```

However, Strings in Python are **immutable** meaning they cannot be changed.
So the expression above doesn’t change name, just like writing 5 + 2 doesn’t
change the value of 5 or 2. So to make sure we keep the result we need to
store it in a variable.

```html

URL = "https://" + name + ".com"
```

So now the variable URL holds the URL created using whatever website name was
given to our function.

### Step 3: Return the URL

Returning a value from a function is simply done using the `return` statement.
Since the variable URL holds the value we want to return, we can write:

```html

return URL
```

to return the value stored in URL. Alternatively, we can skip the step of
saving the value in a variable and put the string addition directly into the
return statement.

```html

return "https://" + name + ".com"
```

### Step 3: Put the pieces of make_address together:

Now that we have all the parts of our function, we can put it together to make
a working function.

```html

def make_address(name):
    URL = "https://" + name + ".com"
    return URL
```

### Step 4: Testing the function:

Now that we’ve created the function `make_address`, we can call it a few times
with different website names to test it. To call a function you write the
function name with values you want to give parameters in parentheses. This can
be done using a **String literal** (any characters between quotation marks
that python reads as a value instead of code) or by putting variable names.

```html

make_address("Google")
```

gives our function the string literal “Google”

```html

site_name = "Facebook"
make_address(site_name)
```

gives our function the value stored in the variable site_name, which is
“Facebook”  
We also need to make sure to print the return value of our function so we can
see if the result is right. The return value can be stored in a variable which
we can then print:

```html

URL = make_address("Google")
print(URL)
```

or we can put the function call inside print and print will use the return
value directly

```html

print(make_address("Facebook"))
```

### Solution:

Now to put it all together, we need to make sure to put the function before we
call the function. Since python reads the lines of your program, calling a
function above the function itself means Python hasn’t seen that function yet,
so as far as Python is concerned it doesn’t exist yet. We also have to make
sure our indentation is correct so the calls to the function `make_address` is
outside of the function.

```html

def make_address(name):
    URL = "https://" + name + ".com"
    return URL

print(make_address("Facebook"))
print(make_address("Google"))
```