## Problem: Below is a dictionary that maps the names of dogs to their breed.
Create a function called `get_breed` that takes the name of a dog and returns
that dog’s breed. If the dog isn’t in the dictionary, return “No dog”. Call
your function twice to test it and print the result: once with a name in the
dictionary and once with a name not in the dictionary.

```html

dogs = {"Callie": "Pitbull", "Sasha": "Jack Russell", "Lexy": "Chihuahua", "Tiny": "Caucasian Shepherd", "Snowball": "Poodle"}
```

## Step 0: Understanding the problem:

This problem gives us a dictionary to use as “global variable”. Here global
means it goes at the top of our python program and is accessible from anywhere
in our program, including in functions. Our task is to create a function that
takes the name of a dog and tries to get the breed of the dog from the
dictionary. If the name isn’t in the dictionary, the function should return
“No dog”

## Step 1: Create a function header:

Our function needs to be called `get_breed` and take a single parameter that
holds a string representing the name of a dog. We’ll simply call this
parameter name:

```html

def get_breed(name):
```

## Step 2: Check for a key in the dictionary:

The first thing we need to do is make sure `name` is in the dictionary. In
python we can do this easily using the `in` keyword. When working with
dictionaries, the expression `k in dictionary` will evaluate to true if the
value stored in k is a key in dictionary. So to check if the dog called `name`
is stored in the dictionary `dogs`, we write

```html

name in dogs
```

If this expression is true, we should get the dog’s breed from the dictionary.
We’ll worry about that later so for now we’ll pass

```html

if name in dogs: 
    pass
```

Otherwise, we need to return “No dog”

```html

if name in dogs: 
    pass
else: 
    return "No dog"
```

## Step 3: Getting a value from the dictionary:

Now that we’ve made sure the name is in our dictionary, we can get the breed
from the dictionary using the name. To do this, we use square brackets with
the key we want to search for.

```html

return dogs[name]
```

## Step 4: Testing our function:

We need to test both cases of our function: when name is in the dictionary and
when it is not. This makes sure that both parts of our if statement work as
they should.

```html

print(get_breed("Tiny"))
print(get_breed("Eric"))
```

## Solution:

```html

dogs = {"Callie": "Pitbull", "Sasha": "Jack Russell", "Lexy": "Chihuahua", "Tiny": "Caucasian Shepherd", "Snowball": "Poodle"}

def get_breed(name): 
    if name in dogs:
        return dogs[name]
    else:
        return "No dog"

print(get_breed("Tiny"))
print(get_breed("Eric"))
```