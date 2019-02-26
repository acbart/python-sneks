# Action Design Research

In the 2019 SIGCSE paper about the Python Sneks curriculum, two experiments were
briefly described. These experiments followed a model of Action Design Research.

> Educational research is frequently confounded by the rapidly changing target
> space and variability between semesters, frustrating efforts to control
> populations for experimental validity. We share the beliefs suggested by
> [Nelson and Ko [21]](https://faculty.washington.edu/ajko/papers/Nelson2018Theory.pdf), that the quest for unarguably valid experimental results
> is a detriment to progress in perfecting designs within computing
> education. The Sneks curriculum is ultimately a design artifact, and
> so frequently decisions were made that could affect the sanctity of
> our experiments. We allowed modifications in a systematic way
> that would contribute to the research space, while acknowledging
> the dynamic nature of educational settings. Therefore, we approach
> our modifications from a Action Design Research (ADR) perspective.
> When ADR is used in an educational setting, the result is
> similar to Instructional Design: an iterative cycle of identifying
> problems in existing curricula, implementing changes, and observing
> the impact. Therefore, the interventions presented in this section
> should be taken with the caveat that the studies are static-group
> comparison designs, and understood for their limitations.

On this page, I have attempted to describe the experiments with more depth than
we could fit in the original 6 pages. Due to time concerns, they were not
described in depth in the SIGCSE presentation. Although hardly ideal, we felt
that this was a better compromise than letting the results not be published.

# Structured Small Groups



Some semi-processed results are available in a [Jupyter Notebook on our GitHub](https://github.com/acbart/python-sneks/blob/master/evaluations/allie-small-groups/research_data_2018.ipynb).

# Worked Examples

**Problem**: Students struggle with difficult programming problems. In particular, a set of problems were selected after the first iteration of the course (Fall 2017) as particularly challenging for students. We initially sorted questions based on their completion rate, and then manually selected a sample from the semester.

Theory: Worked Examples are examples of similar problems, consisting of a "problem formulation, solution steps, and the final answer itself" [25].

Prior work suggests providing Worked Examples with clear subgoal labels could help students deconstruct problems and improve performance [16, 20].

Hypothesis: Providing high quality Worked Examples could help students complete more problems faster and with less stress.

Research Questions:
(1) Do students take advantage of Worked Examples?
(2) Do Worked Examples improve performance?
(3) Do students find Worked Examples helpful?

Intervention: In the second course offering, 8 problems were
selected as the hardest (based on the metric that it took students
longer than average). Worked Examples were created for each
problem and made available to students in the problem prompt.

Data Collection: Quantitative Data was collected via exercise
completion rates and student interaction in the coding platform.
Qualitative Data was collected via a survey on student opinion and
usage of Worked Examples.

Results: Usage of the Worked Examples varied between problems, but roughly 42% of students took advantage of them. Surprisingly, students who took advantage of Worked Examples complete
problems at roughly the same rate as those who did not. Students
who used WEs actually took significantly more time to complete
problems; focusing on students with no prior experience, we see
those that used the WE actually took over twice the time as those
who did not. However, almost 64% of students found the WEs to be
helpful to their learning, with only 18% explicitly disagreeing.

Conclusion: The Worked Examples seemed to have minimal
effect on the completion rate of problems, and possibly even negatively affected students by slowing them down, even though many
students used them and found them helpful.

Limitations:

1. All problems had high completion rates (80-90%) even before introducing Worked Examples.
2. The nonrandom assignment of students in the treatment could hide a more positive effect size.
3. It is possible that our WEs were more like tutorials than WEs
4. It is possible that the benefits of the WEs would have been pronounced on subsequent attempts at related problems.

Some semi-processed results are available in some [Jupyter Notebooks and a poster on our GitHub](https://github.com/acbart/python-sneks/tree/master/evaluations/michael-worked-examples).
