When you run your unit tests, sometimes they fail. The Unittest module that is
running the tests will then attempt to help explain what went wrong.
Sometimes, it gives a Diff Output. Deciphering this output is essential to
using unit tests.

```html

======================================================================
FAIL: test_print_course_info (__main__.MainTest)
----------------------------------------------------------------------
Traceback (most recent call last):
 File "cs1064-f17-fp-version3/test_canvas.py", line 286, in test_print_course_info
 msg="Wrong output for user '{}' in course '{}'.".format(user, course))
AssertionError: '====[50 chars]roups:\n- Exam\n\tWeight: 40%\n\tAssignments: [315 chars].5\n' != '====[50 chars]roups :\n- Exam\n\tWeight: 40%\n\tAssignments:[316 chars].5\n'
 ========== Course Information ==========
- Assignment Groups:
+ Assignment Groups :
?                  +
  * Exam
        Weight: 40%
        Weight: 40%
        Assignments: 1
        Weighted Points: 40.0
[... The rest is cut for brevity ...]
: Wrong output for user 'ron' in course '23'.
```

In the above, we see which function failed, an execution traceback of the
failing line, a helpful Diff Output, and then a message about what went wrong.
In this case, we had the wrong output for the user "Ron" in course 23
("Defense Against the Dark Arts").

In the Diff Output, you will sometimes see that lines start with a "-", a "+",
or a "?":

  * **-** This line was expected, but it was not present (i.e. add this line!)
  * **+** This was not expected, but you put it in anyway (i.e. remove this line!)
  * **?** I have some extra suggestions about this line

So in this case, we got the "Assignment Groups:" line wrong. We were close, so
the Diff put the + and - lines nearby each other. It also added a ? line to
indicate that the problem was an extra space (hence the + on the next line
underneath the space). So

  1. When you see a plus (+), think about removing something
  2. When you see a minus (-), think about adding something.
  3. When you see a question mark (?), think about changing something.

One last thing you will see sometimes are ^ symbols, which indicate you need
to change a character. For example:

```html

Quiz
-     Weight: 15%
? ^        ^
+     Weighf: 15%
? ^^^^     ^
```

In this case, we had to change a set of four spaces to a single tab, and then
we also had to correct a typo (f =&gt; t).