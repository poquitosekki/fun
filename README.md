# Notebooks

Simple notes and takes while playing around with statistics, data science and machine learning topics...

# Introduction to Statistial Thinking

## 1. Introduction to Data

* Case studies
  - So we have 2 groups a treatment group & a control group.
  - Is there a difference in the data?
    * We measure the difference.
    * We spot a difference X between the 2 groups.
    * But this observed X might be just due to chance, and the 2 groups are in fact from the same group.
  - How large should X be to reject the claim that the difference is just due to chance?

* Data Basics
  - Observations, variables and data matrices
    * An observation or case or observational unit is a row in the data matrix
    * A variable is a feature and represents a column in the data matrix
    * Data matrix is NxM table which just holdes N rows (cases) with M columns (set of features)
  - Types of variables
    * Numerical
      - discrete (count)
      - continuous (measure)
    * Categorical
      - nominal (unordered categorical), eg: colors
      - ordinal (ordered categorical), eg: grades (A-F)
  - Relationhips between variables
    * Using a scatterplot we can visualize the relationship between 2 numerical variables
    * 2 variables can either be associated (dependent) or independent.
    * Associations between 2 Variables can be positive or negative.
    * the X variable is the explanatory variables, and the y is the response variable.
    * Just keep in mind that association does not imply causation (Associaton != Causation)
      - the only way to investigate if there is a causal connection is through an experiment!

`TODO: Read more about sampling and experimental design`

* Sampling Principles and Strategies

## 2. Summarizing Data

* Examining numerical data
  - 2 Variables: Scatterplots for paired data (X,Y Numerical variables)
  - 1 Variable: Dotplot provice the most basic display of our data (one variable scatterplot)
  - Histogram: is a simply binned (intervals) version of a stacked dotplot
  - Mean & Weighted Mean
  - Variance & Standard Deviation
    * In practice, the variance and standard deviation are used sometimes to be able to accurately estimate the uncertainty associated with a sample statistic (eg: helps us understand how much a sample mean varies from one sample to the next).
  - Boxplots
  - Quartiles & Median
  - IQR & Variability: the more variable the data, the larger the standard deviation and IQR tend to be.
  - Outliers: observations that appear extreme relative to the rest of the data (out of bound for the whiskers).
    * Preferable to use Robust Statistics (Median,IQR) [Not affected by extreme observations] vs not robust ones (Mean,Sdev)

* Data Transformation 
  - Sometimes the strong skew in data might obscure a lot of potentially useful and interesting details in the data.
  - That's why we do some sort of transformation of our data to make more readable.
  - A transformation is a rescalling of the data using some sort of mapping (function)
  - Most transformation are:
    * Power of 2 & 3
    * Power of 1 = Original Data
    * Log10
    * Sqrt of 2 & 3 (power of 1/2 & 1/3)
    * Power of -1 (1/Data)
    * Power of -1/2 & -1/3
  - Common interests of transforming original data are:
    * seeing the data structure differently
    * reducing the skew
    * assist in modeling (making it easier)
    * straighten a nonlinear relationship in a scatterplot

* Mapping Data
  - Normal plots (dot, scatter, box) sometimes miss the true nature of data, for example when dealing with geographic data it's better to use an intensity map.
  - Intensity maps are not very helpful when it comes to providing precise values, but they shine when want to see some geo-trends.

* Considering categorical data
  - Bar plot
  - Bar plots with 2 Variables
  - Mosaic plots
  - Pie chart

## 3. Probability

## 4. Distributions of random variables

## 5. Foundations of infrerence

## 6. Inference of Categorical data

## 7. Inference of Numerical data

## 8. Introduction to linear regression

## 9. Multiple & Logistic regression
