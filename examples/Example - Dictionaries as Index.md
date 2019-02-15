Lists of dictionaries are a very common nested structure. Often, these
dictionaries will have some kind of ID key that uniquely identifies each
dictionary in the list. Sometimes, we want to quickly find a desired
dictionary given the ID.

```python

users = [{"id": 3, "name": "Klaus", "score": 23},
         {"id": 9, "name": "Pumpkin", "score": 134},
         {"id": 10, "name": "Wrex", "score": 49}]
# How do we quickly get the score of user ID #9?

```

One (bad) solution to this is the following code:

```python

for user in users:
    if user['id'] == 9:
        print(user['score'])

```

This code is bad for two reasons:

  1. Speed: We have to iterate through each and every element to find the desired one. What if there are millions of elements and #9 is the last one?
  2. Readability: Our code is suddenly indented two levels, which makes it harder to read. In Python, we believe that "flat is better than nested".

## Index Dictionary Pattern

Fortunately, dictionaries are here to save our day. We will use the Index
Pattern of dictionaries to speed up our code and make easier to read. The
trick is to create an Index via a dictionary comprehension (which is similar
to a list comprehension):

```python

user_lookup = {user['id']: user for user in users}

print(user_lookup[9]['score'])

```

The `user_lookup` variable will hold a dictionary that maps user IDs to the
user dictionaries themselves. Notice the colon syntax and the curly braces,
which differentiate a dictionary comprehension from a list comprehension. Once
the index is in place, we can quickly jump to the desired user and lookup data
about them.

Using a dictionary as an index is fast - it doesn't matter how many elements
there are in the dictionary, we can jump instantly to right user id. Using the
dictionary is also very readable - no more nesting `if` statements inside of
`for` loops!

## Aligning Lists

This solution becomes even more powerful when we need to align two lists of
related data. Imagine that we have another list of games, and wanted to print
out the player's name and whether they got the problem correct.

```python

problems = [{"user_id": 9, "time", 47, "correct": True},
            {"user_id": 3, "time", 32, "correct": False},
            {"user_id": 9, "time", 29, "correct": False},
            {"user_id": 10, "time", 41, "correct": True}]

```

Aligning these two lists would have been difficult without our index, but now
it's easy!

```python

for problem in problems:
    user_id = problem['user_id']
    user = user_lookup[user_id]
    print(user['name'], problem['correct'])

```

## Summary

Dictionaries being used as indexes are one of the most powerful use cases for
dictionaries, and is just another reason why dictionaries are the best data
structure around!