---
author: "Kyle Jones"
date_published: "March 29, 2024"
date_exported_from_medium: "November 10, 2025"
canonical_link: "https://medium.com/@kyle-t-jones/correlation-and-causation-in-descriptive-statistics-893b5f8f57d0"
---

# Correlation and Causation in Descriptive Statistics Correlation is a relationship between two variables that can be
represented by ordered pairs.

### Correlation and Causation in Descriptive Statistics
Correlation is a relationship between two variables that can be represented by ordered pairs.

#### Correlation Coefficient
Correlation measures how closely two variables are related (a relationship). To see how close these variables are, we work out a correlation coefficient. We would use a test like Spearman's rho (or Pearson's r) to help us find this score.

Correlation is symmetric. It doesn't matter which variable is called X and what is called Y: \`Corr(X,Y) = Corr(Y,X)\`

### Correlation in business analytics
Correlation coefficients measure the strength and direction of the linear relationship between two variables. One of the most commonly used correlation coefficients is Pearson's correlation coefficient, which is also used in linear regression analysis.

#### Facts about correlation coefficient
- Correlation is symmetric: it doesn't matter what variable is called X and what is called Y: \`Corr(X,Y) = Corr(Y,X)\`
- Correlation always falls between −1 and 1
- if r=1 (or r=−1) there is a perfect positive (or negative) LINEAR relationship between X and Y
- If r=0, there is no LINEAR relationship between X and Y but there could be another type of relationship (example: quadratic)
- Strength of correlation is measured by \|𝑟\|, the absolute value of the correlation. For example: a correlation of −0.75 is stronger than a correlation of 0.30 because \|−0.75\|=0.75, which is \> 0.30.

#### Types of Correlation
There are four basic kinds of correlation:

- Negative Linear Correlation: As X increases, Y decreases.
- Positive Linear Correlation: As X increases, Y increases.
- No Correlation: There is not a clear relationship between X and Y.
- Nonlinear Correlation: The rates of change between X and Y are not constant.

### Computing Pearson's Correlation Coefficient
To compute Pearson's correlation coefficient (r) from a dataset of paired x and y values, follow these steps:

1\. Create a table with the x and y values, and add columns for xy, x², and y².

2\. Fill out the xy column by multiplying each x and y value pair.

3\. Fill out the x² column by squaring each x value.

4\. Fill out the y² column by squaring each y value.

5\. Sum the values in each column and put the totals in the bottom row using the Σ notation.

6\. Use this formula to calculate r:

<figcaption>This looks scary but it isn’t. Just go step by step.</figcaption>

Where n is the sample size.

The range of r is between -1 and 1, with:\ 1 means a perfect positive linear relationship \ -1 means a perfect negative linear relationship\ 0 means no linear relationship

#### Interpreting the Correlation Coefficient
The absolute value of r indicates the strength of the linear relationship, with larger values indicating stronger relationships. The sign indicates the direction of the relationship (positive or negative). However, correlation does not imply causation between the variables.

#### Visualizing correlation with scatterplots
A scatterplot represents each observation in the data as an ordered pair (x,y)) of observations on two numeric variables, X and Y. For a sample of n observations, there are n pairs of points. Typically, X is the explanatory variable (also called the independent variable or predictor variable), the "input" that we imagine we can change or manipulate within a mathematical formula. And, Y is the dependent variable, or response variable, the variable that represents the "output" of the mathematical formula.

But remember, the value of the correlation coefficient doesn't change if you look at the correlation between X and Y or the correlation between Y and X.

#### Is the correlation "significant"?
Mathematically, you will always get some value if you provide pairs of values and ask for a correlation. But does that correlation coeffienct matter? Can we trust it?

The t-test for a Correlation Coefficient

How can the t-test be used with a correlation coefficient? We can use a t-test to test whether the correlation between two variables is significant.

<figcaption>Formula for testing the statistical significance of a correlation coefficient.</figcaption>

where r is the test statistic and the t-distribution has n − 2 degrees of freedom

#### Correlation and Causation
Correlation and Causation are not the same thing. Two variables can be correlated and have no connection in the real world. For example, the correlation between the number of layers in California and the amount of money spent on pets is 0.998. This is nearly perfect! But do we believe that a change in one variable changes the other? Is pet spending *causing* more people to be come lawyers? If not, what's going on?

[Tyler Vigen](http://tylervigen.com/view_correlation?id=28671) has a whole book of the spurious (and absurd) correlations. some of them are hilarious. For example, do [Nicolas Cage movies](https://www.tylervigen.com/spurious-correlations) kill people?

<figcaption><a href="https://imgs.xkcd.com/comics/correlation.png" class="markup--anchor markup--figure-anchor" data-href="https://imgs.xkcd.com/comics/correlation.png" rel="nofollow noopener" target="_blank">https://imgs.xkcd.com/comics/correlation.png</a></figcaption>

#### Relationships Between Numeric Variables
In real-world data, we usually gather data on several variables for each observational unit. For example, if studying CEO salaries, we might send a survey to a random sample of CEOs in the US asking them to also report age, years with the company, company sales and profits, etc. Then, we are interested in investigating relationships between variables. There are infinitely many possible relationships. Usually, we care most about how much of a linear relationship they have because more complex relationships can often be captured "locally" by straight lines.

#### Things Analysts Must Consider When Two Variables are Strongly Correlated
1.  [Is there a direct cause-and-effect relationship between the variables?]
2.  [Is there a reverse cause-and-effect relationship between the variables?]
3.  [Is it possible that the relationship between the variables can be caused by other variables?]
4.  [Is it possible that the relationship between two variables may be a coincidence?]

### Related Stories
- [[Confidence Intervals for Business Analytics](https://medium.com/@kylejones_47003/confidence-intervals-c3a1605bfb55)]
- [[Linear Regression for Business Analysis](https://medium.com/@kylejones_47003/linear-regression-for-business-analysis-2407d9fe2942)]
- [[Chi-Squared Test for Independence for Business Analytics](https://medium.com/@kylejones_47003/chi-squared-test-for-independence-a05e53fa5d96)]
