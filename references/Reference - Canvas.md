To simplify accessing the Canvas API, we have provided the `canvas_requests`
module that wraps the `requests` module. In particular, 3 functions are
exposed that let you conveniently access the Canvas website programatically.

As you develop, the system let's you access local test data for three "mocked"
(made-up) users named `'harry'`, `'hermione'`, and `'ron'`. These users have
complete course and user information available.

When you are finished the project, you will be able to use your code to
analyze your own Canvas data. If you want to try this, you will need to obtain
a _Canvas API Token_. These tokens are free and easy to obtain by following
[these
instructions](https://community.canvaslms.com/docs/DOC-10806-4214724194). Once
you have your token (a string of roughly 70 random characters), you can pass
it in to your `main` function instead of `'harry'`, `'hermione'`, or `'ron'`.

![project 6 Server
Diagram](https://vt.instructure.com/courses/66476/files/6800039/download?verifier=pbNNPXSfchCvxPAGJFHguuIXpU3okw8sT7uXePUE&wrap=1)

### get_user

**Description:** The function `get_user` retrieves a User dictionary.

**Syntax:**
```python

canvas_requests.get_user(user_id)
```

**Parameters:**  
\- user_id (`str`): The user_id or token to retrieve a User dictionary for.

**Returns:** `dict`

**Example:**
```python

>>> canvas_requests.get_user("hermione")
{
  # The unique ID of the user
  "id": 42,
  # The full name of the user
  "name": "Hermione Granger",
  # The shortened name of the user
  "short_name": "Hermione Granger",
  # Last name, first name
  "sortable_name": "granger, hermione",
  # Title, if available
  "title": "Student",
  # User-supplied self-description
  "bio": "Interested in Magic, Learning, and House Elf Rights",
  # User-supplied primary email
  "primary_email": "hgranger@hogwarts.edu",
  # University-managed account id
  "login_id": "hgranger@hogwarts.edu",
  # An image URL of the user
  "avatar_url": "https://i.imgur.com/gaNCiuW.png",
  # The users default timezone
  "time_zone": "Europe/London"
}

```

### get_courses

**Description:** The function `get_courses` retrieves a list of Course dictionaries associated with a user (aka the courses they are enrolled in).

**Syntax:**
```python

canvas_requests.get_courses(user_id)
```

**Parameters:**  
\- user_id (`str`): The user_id or token to retrieve courses for.

**Returns:** `list`

**Example:**
```python

>>> canvas_requests.get_courses("hermione")
[
    {
      # The unique ID of the course
      "id": 15,
      # The full name of the course
      "name": "Potions",
      # The current state of the course, one of:
      # 'available', 'unpublished', 'completed', 
      # or 'deleted'
      "workflow_state": "available"
    }, ...
    # Rest redacted
]

```

### get_submissions

**Description:** The function `get_submissions` retrieves a list of Submission dictionaries associated with a user and the course.

**Syntax:**
```python

canvas_requests.get_submissions(user_id, course_id)
```

**Parameters:**  
\- user_id (`str`): The user's name or Canvas token to retrieve courses for.  
\- course_id (`int`): The unique integer ID of the course.

**Returns:** `list`

**Example:**
```python

>>> canavs_requests.get_submissions("hermione", 15)
[
    {
      # The assignment ID that this submission belongs to
      "assignment_id": 270633,
      # The user ID that this submission belongs to
      "user_id": 42,
      # The number of times the assignment was submitted
      "attempt": 1,
      # The raw score assigned to the submission
      "score": 18,
      # When this was submitted. None if unsubmitted.
      "submitted_at": "2017-09-18T21:22:53Z",
      # When this was graded. None if ungraded.
      "graded_at": "2017-09-30T11:43:39Z",
      # The user ID of the grader. None if ungraded.
      "grader_id": 476,
      # Whether the assignment was excused
      "excused": False,
      # Whether the assignment was late
      "late": False,
      # Whether the assignment was missing
      "missing": False,
      # The current status of the submissions. Possible
      # values of "submitted", "unsubmitted", "graded"
      "workflow_state": "graded",
      # A dictionary containing information about the assignment
      "assignment": {
          # The unique ID of the assignment
          "id": 270633,
          # The full name of the assignment
          "name": "#7.5) Programming: Variables and Tracing",
          # The assignment group ID that this assignment belongs to
          "assignment_group_id": 82389,
          # The due date of this assignment (can be None)
          "due_at": "2017-10-10T00:00:00Z",
          # The lock date of this assignment (can be None)
          "lock_at": "2017-09-01T16:40:00Z",
          # The unlock date of this assignment (can be None)
          "unlock_at": None
          # The number of possible points for this assignment (can be None)
          "points_possible": 5.0,
          # A dictionary containing information about the group
          "group": {
              # The unique ID of the group
              "id": 82389,
              # The full name of the group
              "name": "Programming Problems",
              # The assigned weight of this group, relative
              # to other groups. Sums to 100, representing
              # percents.
              "group_weight": 25,
             }
      }
    }, ...
    # Rest redacted
]

```

The information shown here is an abridged version of the [official Canvas
documentation](https://canvas.instructure.com/doc/api/courses.html). You may
find it interesting to review the full API.