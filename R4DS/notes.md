# General Notes 

## Introduction

* What is data science?
  - is a discipline that allows you to turn raw data into understanding, insight and knowledge.

* Model of learning
  - Typical Data science projects follow these steps:
    + Import data (file, database, API...) and load it in a data frame.
    + Tidy the data which means cleaning your data matrix.
    + Transforming data means narrowing down observations, creating new features from existing one (eg: speed from time and distance) and also doing summary statistics. 
      * Tidying + Transforming = Warngling.
    + Visualisation is pretty obvious.
    + Modeling is just using a set of mathematical tools and a set of assumptions concerning the generation of data from a sample or population.
    + Communication is the last step you formalize your results in a way for others to understand them.
  - This [figure](https://d33wubrfki0l68.cloudfront.net/571b056757d68e6df81a3e3853f54d3c76ad6efc/32d37/diagrams/data-science.png) sums up all the steps.
  - We can summarize what we said in: Wrangle, Explore, Model, Communicate.

* Various ideas
  - You can think of visualisation as a tool for hypothesis generation and modeling as a tool for hypothesis confirmation.

## Visualize

* Use [Cheatsheets](https://www.rstudio.com/resources/cheatsheets/)
* Types of plots
  - Scatterplots: ggplot(data=df) + geom\_point(mapping=aes(x=xvar,y=yvar))
  - bar charts  : geom\_bar
  - line charts : geom\_line
  - boxplots    : geom\_boxplot
  - Histogram   : geom\_histogram
  - fitting line: geom\_smooth
* The general underlying Grammar can be summed up into this template with 7 main parameters:
```
ggplot(data = <DATA>) + 
  <GEOM_FUNCTION>(
     mapping = aes(<MAPPINGS>),
     stat = <STAT>, 
     position = <POSITION>
  ) +
  <COORDINATE_FUNCTION> +
  <FACET_FUNCTION>
```
* All the 7 parameters supply what we call the grammar of graphics, a formal system for building plots.

## Transform

* dplyr provides 6 key functions to solve the majority of data manipulation challenges, we can group them into 2 categories:
  - Operations on Rows
        * filter(): pick observations by their values
        * arrange(): reorder rows based on values
  - Operations on columns
        * select(): pick variables by their names
        * mutate(): create new variables using a set of existing ones (or transmute)
  - Various:
        * group_by() and then summarise: getting summaries by group
* Summary functions
  - Measures of location: mean, meadian...
  - Measures of spread: sd, IQR, mad(median absolute deviation)...
  - Measures of rank: min, quantile(x,0.25), max...
  - Measures of position: first(x), nth(x,2), last(x)
  - Counts: n(), sum(!is.na(x)), n_distinct(x), seperate count() function in dplyr

## Explore















