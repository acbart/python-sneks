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

The second experiment was conducted by Michael Friend.

**Problem**: Students struggle with difficult programming problems, spending a fair amount of time/energy and requiring external help to overcome them. 

**Theory**: Worked Examples are examples of similar problems, consisting of a "problem formulation, solution steps, and the final answer itself" ([Skudder and Luxton-Reilly '14](https://dl.acm.org/citation.cfm?id=2667497)). Prior work suggests providing Worked Examples with clear subgoal labels could help students deconstruct problems and improve performance ([Margulieux and Catrambone '14](https://dl.acm.org/citation.cfm?id=2567853), [Morrison et al '15](https://dl.acm.org/citation.cfm?id=2787733)).

**Hypothesis**: Providing high quality Worked Examples could help students complete more problems faster and with less stress.

**Research Questions**:

1. Do students take advantage of Worked Examples?
2. Do Worked Examples improve performance?
3. Do students find Worked Examples helpful?

**Intervention**: In the second course offering, 8 problems were
selected as the hardest (based on the metric that it took students
longer than average) out of the 188 that we were using that semester. Worked
Examples were created for each problem and made available to students in
the problem prompt.

|  | Prior Experience | No Prior Experience | Total |
|-------------|------------------|---------------------|-------|
| Fall 2017 | 240 | 41 | 281 |
| Spring 2018 | 197 | 43 | 240 |
| Total | 437 | 84 |  |

Students had infinite tries over two weeks for each assignment.
They completed the problems in the BlockPy programming environment.
Worked Examples were provided through a separate HTML page that tracked
user behavior.

**Examples**: Here are some examples of our Worked Examples.

* [WE 10- Grade Lookup](https://think.cs.vt.edu/worked_examples/load?filename=10_grade_lookup.html&assignment_id=)
* [WE 11- Heads or Tails](https://think.cs.vt.edu/worked_examples/load?filename=11HeadsOrTails.html&assignment_id=)
* [WE 12- Check Average](https://think.cs.vt.edu/worked_examples/load?filename=12CheckAverage.html&assignment_id=)

**Data Collection**: Quantitative Data was collected via exercise
completion rates and student interaction in the coding platform.
Qualitative Data was collected via a survey on student opinion and
usage of Worked Examples.

**Results**: 

64% of students found the Worked examples helpful, with only 18% explicitly disagreeing.

|  | Prior Experience | No Prior Experience | Total |
|-------------|------------------|---------------------|-------|
| Fall 2017 | 108 | 29 | 137 |
| Spring 2018 | 66 | 12 | 78 |
| Total | 174 | 41 |  |

The addition of Worked Examples provided little to no gain on completion of hard problems

![Completion Rates over Time](sigcse/we_completion_rate.png)

Measured usage of WE varied widely by problem, with an average around 50% of students at least opening them.


| Problem | Percent Usage |
|---------|---------------|
| Cube Elements | 29.4% |
| Default Name | 54.7% |
| Word Frequency | 59.0% |
| Adding Up | 33.3% |
| Plus or Minus | 60.1% |
| Fix Names | 60.5% |
| File Size | 41.2% |

Students who used WEs actually completed the problem in more runs/time than those that didn't.

|  | Used WEs? | Prior Experience? | Mean Number of Runs | StdDev | Mean Time on Task (sec.) | StdDev |
|-----------------------|-----------|-------------------|---------------------|--------|--------------------------|--------|
| Fall 2017 | False | False | 19.5 | 23.3 | 574 | 478 |
|  |  | True | 13.8 | 20.1 | 415 | 393 |
| Spring 2018 (Used WE) | False | False | 7.3 | 7.8 | 311 | 191 |
|  |  | True | 6.6 | 8.3 | 274 | 238 |
| Spring 2018 (No WEs) | True | False | 19.1 | 18.0 | 727 | 476 |
|  |  | True | 17.4 | 19.5 | 707 | 501 |

Focusing on the values for S18 students with no prior experience, we see those that used the WE actually took over twice the time and runs as those who didn't. 
A Cohen's D test gives a large effect size for both measures (p=0.8, p=1.1).

**Conclusion**: The Worked Examples seemed to have minimal
effect on the completion rate of problems, and possibly even negatively affected students by slowing them down, even though many students used them and found them helpful.

**Limitations**:

1. All problems had high completion rates (80-90%) even before introducing Worked Examples.
2. The nonrandom assignment of students in the treatment could hide a more positive effect size.
3. It is possible that our WEs were more like tutorials than WEs
4. It is possible that the benefits of the WEs would have been pronounced on subsequent attempts at related problems.

**Raw Data**: Some semi-processed results are available in some [Jupyter Notebooks and a poster on our GitHub](https://github.com/acbart/python-sneks/tree/master/evaluations/michael-worked-examples).
