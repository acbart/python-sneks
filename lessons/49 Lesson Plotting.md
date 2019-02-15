In this lesson, you will learn how to do basic plotting using the MatPlotLib
module. You can use MatPlotLib to make many kinds of graphs from lists of
data, including line plots, histograms, and scatter plots.

###  &icon-check-plus; Objectives

  1. Create visualizations of data
  2. Intepret visualizations of data
  3. Use the "show" function to correctly render plots
  4. Transform complex nested data into a form suitable for plotting
  5. Choose a suitable graph to answer a question

###  &icon-quiz; Activities

  * [#49) Lesson: Plotting](#video)
  * [#49) Quiz: Plotting](https://vt.instructure.com/courses/66476/assignments/356595)
  * [#49) Programming: Plotting](https://vt.instructure.com/courses/66476/assignments/356688)

###  &icon-educators; Lesson

Download Slides:
[Plotting.pptx](https://vt.instructure.com/courses/66476/files/5919841/download?verifier=rT6vhY4vSeIYVSrWo4VqK90ycBFAPnMfZTrLyNFt&wrap=1
"Plotting.pptx" ){: .instructure_file_link .instructure_scribd_file}

<iframe height="150" width="300" style="width: 640px; height: 480px;"
webkitallowfullscreen="webkitallowfullscreen" title="Plotting"
mozallowfullscreen="mozallowfullscreen"
src="https://www.youtube.com/embed/nkUfeyteVIk?feature=oembed&rel=0"
allowfullscreen="allowfullscreen"></iframe>

&icon-eye; Show/Hide Transcript

**Slide 1 - Plotting:**  
Let's learn about Plotting

**Slide 2 - Visualizations:**  
When you have a large amount of data, you can create visualizations to get a
more intuitive understanding. These visualizations, known as plots or graphs,
take advantage of the fact that humans are good at processing pictures. Making
visualizations in Python is surprisingly easy.

**Slide 3 - MatPlotLib:**  
The most popular library for plotting in Python is named MatPlotLib . As a
very large package, we only need to import only a certain module. For
convenience, we rename that module to be " plt ".

**Slide 4 - Types of Plots:**  
There are 3 kinds of plots that we'll learn about. Each of the plots shown
take in lists of numbers. MatPlotLib actually has many other kinds of plots.
To create other kinds of plots, you can refer to the documentation.

**Slide 5 - Histograms:**  
Although many people find Histograms confusing, they are actually a very
simple kind of plot. They should not be confused with Bar Charts, which are a
more generalized kind of graph. Instead, histograms take a list of numbers and
group them into bins, or ranges of numbers. For example, if we have the list
of numbers shown, we could group them into bins of size 10. Each tick on the
y-axis means another number in that bin. Histograms allow us to see the
distribution or spread of the data.

**Slide 6 - Line Plots:**  
Line plots are another simple kind of graph, and can be used to show a trend
over time or some other factor. Be careful when creating line plots, since
people often use them when a Histogram would be more appropriate.

**Slide 7 - Scatter Plots:**  
When you have two lists of data that you want to match up, a Scatter Plot is
the graph to use. For example, the graph shown here matches students' grade on
a first exam with their grade on a second exam. A scatter plot is used to find
relationships between the two lists of numbers.

**Slide 8 - Labeling:**  
Professional data scientists always label their graphs. MatPlotLib makes it
easy to label the X, Y, and title of the graph. The relevant functions are
xlabel , ylabel , and title, each of which consumes a string.

**Slide 9 - Show:**  
A trick about creating plots is that you need to call the "show" function
afterwards. If you do not call the show function, no graph will appear. A
useful feature of this function is that if you create multiple plots before
showing, these graphs will be combined on the same canvas.

**Slide 10 - Advanced Features:**  
MatPlotLib is an extremely sophisticated library with many, many advanced
features. It is very easy to make legends, adjust colors, more complicated
graphs, and much more. Refer to the MatPlotLib documentation and look up
examples of how to do more with MatPlotLib .

###  &icon-document; Optional Readings

The following readings should be relevant. Remember, all readings are
optional!

###  &icon-flag; Summary

MatPlotLib is a module that can be used to make plots, including line plots,
histograms, and scatter plots.