The following methods all work on string values

# Table of Contents

  * [Table of Contents](#table-of-contents)
  * [Tests](#tests)
    * [count](#count)
    * [endswith](#endswith)
    * [startswith](#startswith)
  * [Changing Case](#changing-case)
    * [title](#title)
    * [capitalize](#capitalize)
    * [upper](#upper)
    * [lower](#lower)
  * [Splitting and Joining](#splitting-and-joining)
    * [split](#split)
    * [join](#join)
  * [Seeking](#seeking)
    * [find](#find)
  * [Whitespace](#whitespace)
    * [strip](#strip)
    * [lstrip](#lstrip)
    * [rstrip](#rstrip)
  * [Editing Strings](#editing-strings)
    * [replace](#replace)
    * [format](#format)

# Tests

These methods allow you to test a string for certain properties; they are
typically used in conditional expressions (e.g., for `if` statements).

## count

**Description**: The method `count` returns the number of times that the `substring` appears in the string `a_string`.  
**Syntax**:
```python

a_string.count(substring)

```

**Parameters**:  
\- substring (`str`): The string to count the number of occurrences of.

**Returns**: `int`  
**Examples**:
```python

> "Harry Potter".count("r")
3
> "Alpha Beta".count("r")
0
> "Hermione Granger".count("P")
0
> new_string = "Hello world"
> new_string.count("l")
2

```

**Full Documentation**:[count](https://docs.python.org/3/library/stdtypes.html#str.count)

* * *

## endswith

**Description**: The method `endswith` returns whether the given string `a_string` ends with the `suffix` string.  
**Syntax**:
```python

a_string.endswith(suffix)

```

**Parameters**:  
\- suffix (`str`): The string that could be at the end of the other string.

**Returns**: `bool`  
**Examples**:
```python

> "Harry Potter".endswith("Potter")
True
> "Hermione Granger".endswith("Potter")
False
> "Treehouse".endswith("House")
False

```

**Full Documentation**:[endswith](https://docs.python.org/3/library/stdtypes.html#str.endswith)

* * *

## startswith

**Description**: The method `startswith` returns whether the given string `a_string` begins with the `prefix` string.  
**Syntax**:
```python

a_string.startswith(prefix)

```

**Parameters**:  
\- prefix (`str`): The string that could be at the beginning of the other
string.

**Returns**: `bool`

**Examples**:
```python

> "Harry Potter".startswith("Harry")
True
> "Hermione Granger".startswith("Harry")
False
> "Treehouse".startswith("tree")
False

```

**Full Documentation**:[startswith](https://docs.python.org/3/library/stdtypes.html#str.startswith)

* * *

# Changing Case

These methods are for changing capitalization in strings.

## title

**Description**: The method `title` returns a new version of the string `a_string` with the first letter of each word capitalized (as you would see in the title of a book).  
**Syntax**:
```python

a_string.title()

```

**Parameters**: None

**Returns**: `str`

**Examples**:
```python

> "This is a full sentence.".title()
'This Is A Full Sentence'
> "hermione granger".title()
'Hermione Granger'
> "WHY AM I SHOUTING".title()
'Why Am I Shouting'

```

**Full Documentation**:[title](https://docs.python.org/3/library/stdtypes.html#str.title)

* * *

## capitalize

**Description**: The method `capitalize` returns a new version of the string `a_string` with only the first letter capitalized. Note that this does not respect periods; only the first letter is capitalized!  
**Syntax**:
```python

a_string.capitalize()

```

**Parameters**: None

**Returns**: `str`

**Examples**:
```python

> "This Is A Title Sentence.".capitalize()
'This is a title sentence'
> "hermione granger".capitalize()
'Hermione granger'
> "WHY AM I SHOUTING".capitalize()
'Why am i shouting'
> "First sentence. Second sentence.".capitalize()
'First sentence. second sentence'

```

**Full Documentation**:[capitalize](https://docs.python.org/3/library/stdtypes.html#str.capitalize)

* * *

## upper

**Description**: The method `upper` returns a new version of the string `a_string` with all of the characters capitalized (uppercase).  
**Syntax**:
```python

a_string.upper()

```

**Parameters**: None

**Returns**: `str`

**Examples**:
```python

> "This Is A Title Sentence.".upper()
'THIS IS A TITLE SENTENCE'
> "hermione granger".upper()
'HERMIONE GRANGER'
> "why am i shouting".upper()
'WHY AM I SHOUTING'

```

**Full Documentation**:[upper](https://docs.python.org/3/library/stdtypes.html#str.upper)

* * *

## lower

**Description**: The method `lower` returns a new version of the string `a_string` with all of the characters lowercase.  
**Syntax**:
```python

a_string.lower()

```

**Parameters**: None

**Returns**: `str`

**Examples**:
```python

> "This Is A Title Sentence.".lower()
'this is a title sentence'
> "Hermione Granger".lower()
'hermione granger'
> "WHY AM I SHOUTING".lower()
'why am i shouting'

```

**Full Documentation**:[lower](https://docs.python.org/3/library/stdtypes.html#str.lower)

* * *

# Splitting and Joining

These methods are for splitting strings into lists or joining sequences (e.g.,
lists) into strings.

## split

**Description**: The method `split` returns a new list by breaking the string `a_string` into elements based on the `separator`.  
**Syntax**:
```python

a_string.split(separator)

```

**Parameters**:  
\- separator (`str`): The string that will be used to find splits. If left
out, this method will instead split on whitespace.

**Returns**: `list` of `str`

**Examples**:
```python

> "Harry Potter, Hermione Granger, Ron Weasley".split(',')
['Harry Potter', ' Hermione Granger', ' Ron Weasley']
> "and/or".split("/")
['and', 'or']
> "There will be no splits.".split("-")
['There will be no splits.']
> "".split("Empty string")
['']
> "Leaving out the argument will split on all whitespace!".split()
['Leaving', 'out', 'the', 'argument', 'will', 'split', 'on', 'all', 'whitespace!']

```

**Full Documentation**:[split](https://docs.python.org/3/library/stdtypes.html#str.split)

* * *

## join

**Description**: The method `join` returns a new string by combining the elements of `a_sequence` using `a_string`.  
**Syntax**:
```python

a_string.split(a_sequence)

```

**Parameters**:  
\- a_sequence (`list` of `str` or other sequence of `str`): The sequence of
strings that will be joined together. You must make sure these are strings!

**Returns**: `str`

**Examples**:
```python

> ','.join(['Harry Potter', 'Hermione Granger', 'Ron Weasley'])
'Harry Potter,Hermione Granger,Ron Weasley'
> "/".join(["and", "or"])
'and/or'
> "Nothing to join together".join([])
''
> "".join(["No", "Spaces", "Or", "Anything"])
''NoSpacesOrAnything'

```

**Full Documentation**:[join](https://docs.python.org/3/library/stdtypes.html#str.join)

* * *

# Seeking

These methods are used to look through a string and find positional
information.

## find

**Description**: The method `find` returns the numerical index of the first appearance of `substring` in `a_string`. Remember, counting starts at 0. If the substring is not in the string, then `-1` is returned.  
**Syntax**:
```python

a_string.find(substring)

```

**Parameters**:  
\- substring (`str`): The string to find in `a_string`.

**Returns**: `int`

**Examples**:
```python

> "Harry Potter".find('r')
2
> "Capitalization is Important".find('I')
18
> "Harry Potter".find('g')
-1
> "".find('e')
-1
> "You can check for more than one character!".find("can")
4

```

**Full Documentation**:[find](https://docs.python.org/3/library/stdtypes.html#str.find)

* * *

# Whitespace

These methods remove whitespace from strings (spaces, tabs, new lines, etc.).

## strip

**Description**: The method `strip` returns a new string with any whitespace (e.g., spaces or tabs) removed from both sides.  
**Syntax**:
```python

a_string.strip()

```

**Parameters**: None

**Returns**: `str`

**Examples**:
```python

> "      Garbage whitespace     ".strip()
'Garbage whitespace'
> "Works on either side      ".strip()
'Works on either side'
> "Common task is to remove newlines\n\n".strip()
'Common task is to remove newlines'

```

**Full Documentation**:[strip](https://docs.python.org/3/library/stdtypes.html#str.strip)

* * *

## lstrip

**Description**: The method `lstrip` returns a new string with any whitespace (e.g., spaces or tabs) removed from only the LEFT side.  
**Syntax**:
```python

a_string.lstrip()

```

**Parameters**: None

**Returns**: `str`

**Examples**:
```python

> "      Garbage whitespace".lstrip()
'Garbage whitespace'
> "Works on one side only     ".lstrip()
'Works on one side only     '

```

**Full Documentation**:[lstrip](https://docs.python.org/3/library/stdtypes.html#str.lstrip)

* * *

## rstrip

**Description**: The method `rstrip` returns a new string with any whitespace (e.g., spaces or tabs) removed from only the RIGHT side.  
**Syntax**:
```python

a_string.rstrip()

```

**Parameters**: None

**Returns**: `str`

**Examples**:
```python

> "Garbage whitespace     ".rstrip()
'Garbage whitespace'
> "     Works on one side only".rstrip()
'     Works on one side only'

```

**Full Documentation**:[rstrip](https://docs.python.org/3/library/stdtypes.html#str.rstrip)

* * *

# Editing Strings

This method is used to conveniently edit strings.

## replace

**Description**: The method `replace` returns a new string based on `a_string`, but with any occurrence of `old` replaced by `new`.  
**Syntax**:
```python

a_string.replace(old, new)

```

**Parameters**:  
\- old (`str`): The original text to find in the string.  
\- new (`str`): The new text to change the `old` text into.

**Returns**: `str`

**Examples**:
```python

> "Can you open the door?".replace("open", "close")
'Can you close the door?'
> "Multipl? occurr?nc?s".replace("?", "e")
'Multiple occurrences'
> "Useful for e-r-a-s-i-n-g too!".replace("-", "")
'Useful for erasing too!'

```

**Full Documentation**:[replace](https://docs.python.org/3/library/stdtypes.html#str.replace)

* * *

## format

**Description**: The method `format` returns a new string based on `a_string`, but with the parameters added in to replace any `{}` with any number of parameters given in `args`.  
**Syntax**:
```python

a_string.format(*args)

```

**Parameters**:  
\- args (Any type): 0 or more values that will be injected into `a_string`,
replacing any occurrences of `{}` in order.

**Returns**: `str`

**Examples**:
```python

> "The sum of 1+1 is {}".format(2)
'The sum of 1+1 is 2'
> "{} arguments can be {}".format("Multiple", "passed")
'Multiple arguments can be passed'

```

**Full Documentation**:[format](https://docs.python.org/3/library/stdtypes.html#str.format)

* * *