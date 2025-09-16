---
title: Chapter 1
---

## 1.1 Sampling

### Population
Collection of objects or outcomes about which information is sought

#### Tangible populations
Population consisted of physical objects

#### Conceptual population
All the values that might possibly have been observed. And infinite population
Could be the measurements of a determined experiment.

### Sample
Subset of a population, containing the objects or outcomes that are actually observed

#### Simple random sample
Sample of size _n_ chosen by a method in which each collection of _n_ population items is equally likely to make up the sample

The items in a random sample are considered to be independent except when the population is finite and the sample is larger than 5%

#### Sample of convenience
Sample that is obtained in some convenient way. For example the top bricks in a pile

#### Independent
The items in a sample are said to be independent if knowing the values of some of them does not help to predict the values of the others

#### Weighted sampling
Sampling where some items are given a greater chance of being selected

#### Stratified random sampling
The population is divided into subpopulations (strata) and a simple random is drawn from each group

#### Cluster sampling
Items are drawn from the population in groups

For example, to measure sociological factors in a country


### Experiments

#### One-sample
One population of interest and a single sample is drawn from it

#### Multisample
Two or more populations of interest and a sample is drawn from each population

#### Factorial
A [[chapter1.md#multisample]] experiment is distinguished from one another by the varying of one or more factors that may affect the outcome

#### Controlled experiment
The process can be run several times, changing a factor. The values of the factor are under the control of the experimenter

#### Observational study
The experimenters cannot control the factors


### Types of data

#### Numerical (quantitative)
How much or how many its assigned to each item in a sample

#### Categorical (qualitative)
Items are placed into categories


## 1.2 Summary Statistics

### Sample Mean
Called the __arithmetic mean__ or __average__  is a measure of center, sensible to outliers
$$
\overline{x} = \frac{1}{n} \sum_{i=1}^{n} X_i
$$

### Sample variance
The average of the squared deviations

$$
s^2 = \frac{1}{n-1}\sum_{i=1}^{n}(x_i-\overline{x})^2
$$

### Sample standard deviation
The square root of the variance

$$
s = \sqrt{\frac{1}{n-1}\sum_{i=1}^{n}(x_i-\overline{x})^2}
$$

### Sample median
Measure of center, not sensible to outliers. Is the middle number

- If _n_ is odd, the median is the number in the position $$ \frac{n+1}{2} $$
- If _n_ is pair, the median is the average of the numbers in positions $$ \frac{n}{2} $$ and $$ \frac{n}{2} + 1 $$


### Trimmed mean
A less sensitive to outliers mean. Arrange the values in order and _trimming_ an equal number of items from each end and computing the mean of those remaining

Common used trimmings are: _5% 10% 20%_


### Mode
Most frequently occurring value

### Range
Difference between the largest and smallest values in a sample


### Quartiles
Divide a sample as nearly as possible into quarters. A sample has 3 quartiles:

- 0.25(n+1)
- 0.4(n+1)
- 0.75(n+1)

### Percentiles
The pth percentile of a sample, for a number p between 0 and 100, devides the sample so that as nearly as posible p% of the sample values are less than the pth percentile and (100-p)% are greater

$$
(\frac{p}{100})(n+1)
$$

The first quartile is the 25th percentile, the median is the 50th percentile and the third quartile is the 75th percentile

### Frequencies
Number of sample items that fall into a category

### Relative Frequencies (sample proportions)
Is the frequency divided by the sample size


## 1.3 Graphical Summaries

### Steam and leaf plot
Each item in the sample is divided into two parts: a steam, consisting of the leftmost one or two digits, and the leaf, which consists of the next digit

![steam and leaf plot](./static/steam-leaf-plot.png)

### Dotplots
Can be used to give a rough impression of the shape of a sample. Useful when the sample size is not too large

![dotplot](./static/dotplot.png)

### Histogram
Graphic that gives an idea of the "shape" of a sample, indicating regions where sample points are concentrated and regions were they are sparse

#### Frequency table
Table with class-intervals in the left-hand column which divide the sample into groups, usually with the same width. Next they have the frequency, the relative frequency (frequency/sample size) and the density (relative frequency/interval width)

![frequency table](./static/frequency-table.png)

#### Chart
The x axis denotes the classes and the y could be the frequency, relative frequency or density when all the classes are the same width, however, if any class has a different width, the density is need to be used

![histogram](./static/histogram.png)

#### Symmetry
A histogram is symmetric if its right half is a mirror image of its left half

![symmetry](./static/symmetry.png)

#### Skewness
A histogram that is not symmetric is skewed

Could be left skewed

![left](./static/left.png)

Or right skewed

![right](./static/right.png)

## Boxplots
Graphic that represents the median, the first and third quartiles, and any outliers that are present in a sample

![IQR](./static/iqr.png)

### Interquartile Range
The interquartile range is the difference between the third quartile and the first quartile
If a value is gratter than the third quartile plus 1.5*IQR or lower than the first quartile minus 1.5*IQR is said to be an outlier

