The dictionary counting pattern is a useful way to count occurrences in a
list, when you don't know all the categories of things upfront. A dictionary
is used to keep track of occurrences, using the items in the list as keys. The
dictionary summing pattern is based on the same idea, and can be particularly
useful when you combine it with a richer data structure like a list of
dictionaries. Notice that there are now two kinds of dictionaries in play: the
summing dictionary (your accumulator) and the dictionaries being processed
from a list.

## Starting Data

Assume we have a list of dictionaries representing a large number of movies:

```python

movies = [{"Name": "Harry Potter", "Genre": "Fantasy", "Length": 159},
          {"Name": "Star Wars", "Genre": "Sci-Fi", "Length": 152},
          {"Name": "Narnia", "Genre": "Fantasy", "Length": 150},
          {"Name": "Blade Runner", "Genre": "Sci-Fi", "Length": 117},
          {"Name": "2001: A Space Odyssey", "Genre": "Action", "Length": 161},
          {"Name": "It", "Genre": "Horror", "Length": 187},
          ...]

```

## Dictionary Initialization

And you want to know the total running length of all the movies, but in each
genre. A dictionary can be used to keep track of each genre's sum. We
initalize the dictionary to be empty.

```python

lengths = {}

```

## Iteration

Then we iterate through each movie dictionary to process them one-at-a-time.

```python

for movie in movies:
    ...

```

## Check for New Category

We check if we have the seen the movie's genre before - if we have not, we
will need to create an entry for it. Notice how we use the movie's genre as a
key for the dictionary - recall that the expression will be substituted for an
actual value at runtime!

```python

if movie['Genre'] not in lengths:
    lengths[movie['Genre']] = 0
<p/pre>
```

## Update Category

Then, we can safely increase the value associated with that genre by the
length for that movie.

```python

lengths[movie['Genre']] += movie['Length']

```

## Print Result

Once all is said and done, we can iterate through the genre/length pairs and
print out their values:

```python

for genre, length in lengths.items():
    print(genre, length)

```

## Final Solution

Putting all of this code together:

```python

movies = [{"Name": "Harry Potter", "Genre": "Fantasy", "Length": 159},
          {"Name": "Star Wars", "Genre": "Sci-Fi", "Length": 152},
          {"Name": "Narnia", "Genre": "Fantasy", "Length": 150},
          {"Name": "Blade Runner", "Genre": "Sci-Fi", "Length": 117},
          {"Name": "2001: A Space Odyssey", "Genre": "Action", "Length": 161},
          {"Name": "It", "Genre": "Horror", "Length": 187},
          ...]

lengths = {}
for movie in movies:
    if movie['Genre'] not in lengths:
        lengths[movie['Genre']] = 0
    lengths[movie['Genre']] += movie['Length']

for genre, length in lengths.items():
    print(genre, length)

```