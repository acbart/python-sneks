What is proper code organization? If you search on Google, you will find many
guides and articles about how to organize code well, so opinions will vary.
There's an [official Python style guide
(Pep8)](https://www.python.org/dev/peps/pep-0008/) and organizations like
[Google have their own official style
guides](https://google.github.io/styleguide/pyguide.html). There are even
tools that you can use to test if your program has good style, like
[pylint](https://www.pylint.org/). Later in your careers, you may find people
have other opinions. But for this project, here are the things I'm thinking
about when I talk about good style.

### Bad Variable Names

Variable names are critically important, and naming is more of an art than a
science. You want to make names that are clear, concise, and accurate. Here
are some common ways that variable names go wrong:

  * Names that are too long (`thing_that_I_am_looking_for_right_now`)
  * Trivially short names (`r` or `ab`). Note that a name like `x` is an okay name if you are talking about an x-coordinate, but bad if you are talking about anything else.
  * Unclear abbreviations (`crs_grp` instead of `course_group`), although sometimes its okay if it is one that everyone knows (`pid` instead of `private_identifier`).
  * Misleading name (naming a variable holding a list of courses as `banana_pudding`) or bad hungarian notation (an integer variable named `my_list`). Note that you don't need to use hungarian notation, where you add the type of the variable to the name, it is simply one stylistic option.

### Good Documentation

Some people refuse to add documentation to their programs. Some people tell
you to document every line. The best reality is somewhere in-between. Here are
the three cases I like to document:

  * Start of File: Whenever you create a new project, it helps to add a few lines at the top explaining what it does.
  * Functions: Whenever you create a function, either because an instructor told you to or because it made your life easier, you should document it. Describe what it does, what it consumes, and what it returns. If there are particularly surprising features of the function (_"If you run this function multiple times, your computer might catch on fire"_), this is a good place to mention it.
  * Large chunks of code: Often, we put large chunks of code into functions and give those functions clear, concise names. But sometimes we don't have that option, for one reason or another. A good compromise is to document a chunk of code with a clear comment explaining what it does (_`# Calculate a running sum"` _).
  * Weird code: We always try to make code as clear as possible, but sometimes we are forced to write something very weird. If you struggled to write it, someone will probably struggle to read it. Leave a comment above to remind your future self and coworkers what it does.

As an example of documenting function, let's document a function for
processing lists of numbers:

```python

def add_up(numbers, weight):
    """
    Adds together a sequence of numbers, multiplying each one by a constant weight.
    Args:
        numbers (list of int): A sequence of numbers
        weight (int): A single number to be multiplied against the others
    Returns:
        int: A single number representing the total value.

```

This example follows the [Google DocString format](http://sphinxcontrib-
napoleon.readthedocs.io/en/latest/example_google.html).

### Helper Functions

If you've written the same chunk of code 3 times, odds are good that it can be
extracted into a function. This will reduce the length of your code, and the
number of opportunities for a typo to slip in.

### Extreme Nesting

A famous Pythonista once said, _"Flat is better than nested."_ Wherever we
can, we avoid indenting (i.e. using unnecessary `for`, `if`, etc.). Sometimes,
we cannot avoid it. But if there's a better way, we often go for it. For
example, aligning lists of dictionaries can be done more efficiently with a
dictionary index than with a nested for/if loop.

### Excessive Line Length

Terminal windows used to be 80 characters long. Even though we have bigger
screens, most programmers still try to limit their line widths to 80
characters, out of respect for those with older machines or smaller monitors.
Most environments (including Spyder) will show a grey bar at the 80 character
limit.

### Excessive Function Height

It's unavoidable sometimes, but functions that go on for hundreds of line are
typically out of control and need to be broken up using helper functions.

### Consistent Style

Everyone has their own coding style, but you should be consistent with your's.
Here are two particular places to consider:

  * Variable names: Python prefers using `snake_case` (underscores) instead of `camelCase` (mixture of upper and lower case) to replace spaces in variable names. You are not required to use one, but you must be consistent.
  * Whitespace: Should you put spaces after parentheses (`print( test )` vs. `print(test)`? After numerical operators (e.g. `5+5` vs. `5 + 5`)? The choice is your's, but be consistent.

### Messy Code

We often try to solve a problem in multiple ways, before finding a final
solution. If you are commenting out old code, put it in a separate file or
delete it. You should not have tons of old dead code littering up your file.

### Bad Imports

Imports, stylistically, belong at the top of a file. Do not place them
throughout a program, unless you MUST (and you almost never need to). Also,
make sure you are not importing packages that you then never use.