![example_output.png](https://vt.instructure.com/courses/66476/files/5919887/download?verifier=vWivadJlXOQXqmiZFc0jfddqi87clsa5ouN7H9NK&wrap=1)

The Grade Trend plot shows how a students' grade evolves over the semester.
The first half of the graph shows progress so far in the course, while the
second half shows what could happen with any ungraded assignments. The top-
most line ("Maximum") shows the maximum points that were possible over the
entire semester, ignoring the student's actual score. The two other lines
represent the student's "Highest" and "Lowest" possible scores. These two
lines are the same until the point in the semester where there are ungraded
assignments, at which point they fork into two paths. The top path assumes the
student receives a perfect on every remaining assignment, and the bottom path
assumes they get a zero on the remaining assignments.

Although this may seem complicated, it is straightforward as long as you
translate each step carefully.

### Formula

Here are some shorthand formula to break down exactly how the three plots are
calculated:

```python

(max_points of a submission) = 100 * (points_possible of submission) * (group_weight of submission)
total_max = sum(max_points/100)

(low_score of a submission) = 0 if submission is not graded,
                              otherwise (score of submission)
(low_points of a submission) = 100 * (low_score of submission) * (group_weight of submission)

(high_score of a submission) = (points_possible of submission) if submission is not graded, 
                               otherwise (score of submission)
(high_points of a submission) = 100 * (high_score of submission) * (group_weight of submission)

Calculate the running sum of low_points as a series
Calculate the running sum of high_points as a series
Calculate the running sum of max_points as a series

Divide each element of the running sums by the total_max

Plot each running sum series

```

### Example

These formula are tricky, so let's look at an example for a course with 4
potential submissions (2 of which have been graded, and 2 of which have not
been graded):

| score | workflow_state | points_possible | group_weight  
---|---|---|---|---  
1 | 5 | "graded" | 10 | 20  
2 | 2 | "graded" | 2 | 40  
3 | None | "submitted" | 5 | 20  
4 | None | "submitted" | 6 | 40  
  
We'll be iterating through these **4** submissions (and their associated
assignment and group) and need to do several rounds of calculation.

  
**First**, we'll calculate the max_points, low_points, and high_points for each independent submission:

| max_points | low_points | high_points  
---|---|---|---  
1 | 100*10*20=20,000 | 100*5*20=10,000 | 100*5*20=10,000  
2 | 100*2*40=8,000 | 100*2*40=8,000 | 100*2*40=8,000  
3 | 100*5*20=10,000 | 100*0*20=0 | 100*5*20=10,000  
4 | 100*6*40=24,000 | 100*0*40=0 | 100*6*40=24,000  
  
Notice that for graded assignments, the low_points and high_points are the
same; for ungraded assignments, the max_points and high_points are the same
(and low_points are zero).

**Second**, we'll calculate the maximum score by adding up all the max_points and dividing by 100:

max_points = (20,000 + 8,000 + 10,000 + 24,000)/100 = 620

**Third**, we'll calculate the running the sums:

| running_max | running_low | running_high  
---|---|---|---  
1 | 0+20,000=20,000 | 0+10,000=10,000 | 0+10,000=10,000  
2 | 20,000+8,000=28,000 | 10,000+8,000=18,000 | 10,000+8,000=18,000  
3 | 28,000+10,000=38,000 | 18,000+0=18,000 | 18,000+10,000=28,000  
4 | 38,000+24,000=62,000 | 18,000+0=18,000 | 28,000+24,000=52,000  
  
**Fourth**, we'll divide each element of the running sums by the max_points, to get our final values:

| maxes | lows | highs  
---|---|---|---  
1 | 20,000/620=32.3 | 10,000/620=16.1 | 10,000/620=16.1  
2 | 28,000/620=45.2 | 18,000/620=29.0 | 18,000/620=29.0  
3 | 38,000/620=61.3 | 18,000/620=29.0 | 28,000/620=45.2  
4 | 62,000/620=100 | 18,000/620=29.0 | 52,000/620=83.9  
  
**Finally**, the values above are the ones we end up plotting.

There were many ways to arrange these calculations. However, you can't do this
in one loop: you will need to do multiple rounds of iteration when all is said
and done.

### General Running Sum Pattern

```python

# Initialize
running_sum = 0
running_sums = []
# Iterate
for item in a_list:
    # Update
    running_sum = running_sum + item
    running_sums.append(running_sum)

```