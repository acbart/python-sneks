## Problem: Create a function `convert_to_feels` that consumes a number
(representing a temperature) and returns `"hot"` if it is above 70, `"cold"`
if is below 50, and `"comfortable"` otherwise.

Then, create a function `map_feels` that consumes a list of numbers
(representing temperatures) and returns the list with each temperature
converted to strings `"hot"`, `"cold"`, and `"comfortable"` (by using
`convert_to_feels`).

Test convert_to_feels by calling it with a number and printing the result.
Test map_feels by calling it with a list of numbers and printing the result.

## Step 0: Understanding the problem:

This question may seem like a lot to take in, but if we break it down into its
parts we see it’s not too bad.

First it asks us to write the function `convert_to_feels`. All this function
has to do is take in a number that represents a temperature and return a
string describing the temperature (either hot, cold, or comfortable). This
function can be done using an if statement on the number given. Then we have
to test this function by calling it and printing the result.

Then it asks us to write the function `map_feels` that takes a list of numbers
and returns a new list of the strings that represent the numbers in the given
list. This is made easier with `convert_to_feels` because we can just call
`convert_to_feels` on each number to get the string representation. Since we
need to perform an operation on a list of values, we should use a for loop. We
have to test this function by calling it with a list of numbers and printing
the result.

## Step 1: Creating the function header

Based on our practice from previous examples, we can create the header for the
function `convert_to_feels` that takes a single number:

```html

def convert_to_feels(temp):
```

And the function `map_feels` that takes a list of numbers:

```html

def map_feels(temp_list):
```

## Step 2: Writing `convert_to_feels`:

## Step 2a: Creating an if statement (for `convert_to_feels`):

Our function `convert_to_feels` is meant to capture the following logic:

```html

If temp is above 70,
    return hot
If temp is below 50,
    return cold
Otherwise
    return comfortable
```

We can implement this logic in our function by simply using an if-elif
structure:

```html

if temp > 70:
    return "hot"
elif temp < 50:
    return "cold"
else: 
    return "comfortable"
```

## Step 2b: Creating the function:

Now that we have an if statement that does what our `convert_to_feels`
function is meant to do, we can put it into our function.

```html

def convert_to_feels(temp):
    if temp > 70:
        return "hot"
    elif temp < 50:
        return "cold"
    else: 
        return "comfortable"
```

## Step 3: Writing `map_feels`:

## Step 3a: Creating an empty list

Since we need to build a list of strings that correspond to each number in
`temp_list`, we need to create a new, empty list to hold the values as we
generate them:

```html

feels_likes = []
```

## Step 3b: Creating the for loop:

We need to go through each entry in the list we are given and convert the
temperature number to a feels string. We can do this with a simple for-each
loop, like this:

```html

for temp in temp_list:
    # Do something
```

The meaning of this for-each loop is relatively straightforward, it means “for
each temp in temp_list, do something”, now we just have to figure out what
“something” is.

## Step 3c: Use function to get a value and add to a list:

For every number in `temp_list`, we need to get the feels like string and add
it to our `feels_likes` list. To get the feels like string, we can use our
`convert_to_feels` function, passing it the number we are currently working
with. In a for-each loop, the thing before the `in` keyword is called the item
variable. In our case the item variable is `temp`. This variable is created
just for the loop and is given each of the values in our list one at a time.
Each time the item variable gets a new value, the “Do something” part of the
loop, called the is called. So if there is something we want to do to every
value in the list, we can put it inside the loop and assume the variable
`temp` holds some value in our list.

For this problem, we need to use the `convert_feels` function to get the feels
like string of temp, then add the string to `feels_likes`. To add to the end
of the `feels_like` list, we simply use the `append()` function on the list:

```html

feels_likes.append(some_value)
```

But instead of some_value, we need to add the result of calling
`convert_to_feels` on temp:

```html

feels_likes.append(convert_to_feels(temp))
```

## Step 3d: Putting the loop together:

Now that we have the parts of our loop, we can put it together:

```html

for temp in temp_list:
    feels_likes.append(convert_to_feels(temp))
```

## Step 3e: Putting the function together:

Now we can put everything we built in previous steps into our function:

```html

def map_feels(temp_list): 
    feels_likes = [] 
    for temp in temp_list:
        feels_likes.append(convert_to_feels(temp))
```

All that we have left to do is return the feels_likes list once the loop is
finished. Make sure to put the return statement on the outside of the loop.
Once a function reaches a return statement it is finished, so if we put the
return statement on the inside of the loop our loop would run once, hit the
return statement, then return and be finished.

```html

def map_feels(temp_list): 
    feels_likes = [] 
    for temp in temp_list:
        feels_likes.append(convert_to_feels(temp))
    return feels_likes
```

## Step 4: Testing our functions:

Now that both functions are written, we need to make sure they work properly.

First we should test the `convert_to_feels` function since `map_feels` uses
it, so if `convert_to_feels` doesn’t work, neither will `map_feels`.

```html

print(convert_to_feels(45))
```

Now that we know `convert_to_feels` works, we can test `map_feels`

```html

print(map_feels([50, 90, 30])
```

## Solution:

```html

def convert_to_feels(temp):
    if temp > 70:
        return "hot"
    elif temp < 50:
        return "cold"
    else: 
        return "comfortable"

def map_feels(temp_list): 
    feels_likes = [] 
    for temp in temp_list:
        feels_likes.append(convert_to_feels(temp))
    return feels_likes

print(convert_to_feels(45))
print(map_feels([50, 90, 30]))
```