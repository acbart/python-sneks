## 0) Read Problem

Write a function called `count_pets` that consumes a list of strings of pet
types owned and returns the number of each type of pet as a dictionary. Use
the Dictionary Counting pattern. Call your function with the following list to
test it.

```html

["Dog", "cat", "Cat", "Snake", "mouse", "snake", "dog", "dog"]
```

Notice the list is written somewhat sloppy. The capitilization is
inconsistent. Your function needs to be able to fix this so that “Dog” and
“dog” go into the same dictionary entry.

## 1) Interpret the Problem

This problem requires us to write a function that uses the Dictionary Counting
pattern to create a dictionary that maps pet type to number of pets of that
type. The problem also says the words in the list can have inconsistent
capitalization and our function has to treat two of the same word as one key
in the dictionary.

## 2) Write Test

Once we understand the problem, it helps to think of the possible cases we can
test. If we do these first, we can run our code as we go to make sure we’re
catching every possibility.

Here is a basic case with a list of strings with consistent capitalization.

```html

pets1 = ["dog", "cat", "snake", "dog", "lizard", "cat", "cat"]
print(count_pets(pets1))
# => "{"DOG": 2, "CAT": 3, "SNAKE": 1, "LIZARD": 1]
```

The case given in the problem, where the capitalization is inconsistent

```html

pets2 = ["Dog", "cat", "Cat", "Snake", "mouse", "snake", "dog", "dog"]
print(count_pets(pets2))
# => "{"DOG": 3, "CAT": 2, "SNAKE": 2, "MOUSE": 1]
```

A case with an empty list

```html

print(count_pets([])
# => "{}"
```

## 3) Create function header

Our function should be called `count_pets` and take 1 parameter. The parameter
holds a list of strings representing types of pets so a good name would be
`pets`

```html

def count_pets(pets): 
    ...
```

## 4) Initialize the Dictionary

The first thing we need to do is create a dictionary to add entries to

```html

pets_count = {}
```

## 5) Iterate over the list

To check at each entry in the pets list, we should use a for loop. This for
loop will look at every string in the list, one at a time. The “item” variable
is the variable that will hold each value in the list as your loop repeats.
Since we have a pets list, we should name our item variable pet.

```html

for pet in pets:
    ...
```

## 6) Normalizing Strings

Since the strings in the list could have inconsistent capitalization, we need
a way to “normalize” the data. In programming, “normalize” usually means to
take data that is in some way inconsistent and change it in a way that makes
it easier to process.

The easiest way to normalize strings that have inconsistent capitalization is
to change them all to the same capitalization. This can be done using the
`upper` or `lower` functions that return the string in all caps and all
lowercase, respectively. Since `"Dogs".upper()` is `"DOGS"` and
`"dogs".upper()" is also`“DOGS”`, these two strings can now be seen as the
same.

It doesn’t matter which of these we use, so we’ll use `upper`. We’ll save this
uppercase string in a new variable to use later.

```html

petUpper = pet.upper()
```

## 7) Implementing the Dictionary Count Patter

Now we need to update our dictionary for each pet using the Dictionary Count
pattern. If the dictionary already contains a key matching the current pet, we
should increment the value of the counter value for that key.

```html

if petUpper in pets_count:
    pets_count[petUpper] = pets_count[petUpper] + 1
```

If the key doesn’t exist, we should create it and give its counter value an
initial value of 1

```html

if petUpper in pets_count:
    pets_count[petUpper] = pets_count[petUpper] + 1
else: 
    pets_count[petUpper] = 1
```

Notice we use petUpper as the key. This makes sure that we’re not adding “dog”
and “Dog” as separate keys. Both string will become a single key “DOG”.

## 8) Returning the Result

Once our loop finishes, all we have left to do is return the resulting
dictionary

```html

return pets_count
```

## Solution

With all the pieces put together we get our solution, which passes the tests
we wrote when run!

```html

def count_pets(pets): 
    pets_count = {}
    for pet in pets:
        petUpper = pet.upper()
        if petUpper in pets_count:
            pets_count[petUpper] = pets_count[petUpper] + 1 
        else: 
            pets_count[petUpper] = 1

    return pets_count

# Tests
pets1 = ["dog", "cat", "snake", "dog", "lizard", "cat", "cat"]
print(count_pets(pets1))
# => "{"DOG": 2, "CAT": 3, "SNAKE": 1, "LIZARD": 1]

pets2 = ["Dog", "cat", "Cat", "Snake", "mouse", "snake", "dog", "dog"]
print(count_pets(pets2))    
# => "{"DOG": 3, "CAT": 2, "SNAKE": 2, "MOUSE": 1]

print(count_pets([])
# => "{}"
```