# Introduction to Data Science

## Top

[Learning Targets](#learning-targets)

[R Programming](#r-programming)

[Data Collection and Organization](#data-collection-and-organization)

[Descriptive Statistics](#descriptive-statistics)

[Math Medic](#math-medic)

[DeltaMath](#deltamath)

## Learning Targets

[LT00: Digital Citizenship & Collaboration](https://lms.lausd.net/page/7685035866)  
[LT01: Claim, Evidence, Reasoning, Evaluate, Critique (CER & EC)](https://lms.lausd.net/page/7685074399)  
[LT02: Critical Digital Researcher](https://lms.lausd.net/page/7689272471)  
[LT03: Data Storage and Privacy](https://lms.lausd.net/page/7707538554)  
[LT04: RStudio Functions & Syntax](https://lms.lausd.net/page/7707542186)  
[LT05: RStudio Dataset Manipulations](https://lms.lausd.net/page/7707592976)  
[LT06: One-Variable Plots](https://lms.lausd.net/page/7707610259)  
[LT07: Multivariable or Complex Plots](https://lms.lausd.net/page/7707616357)  
[LT08: Interpreting Numerical Data](https://lms.lausd.net/page/7707618017)  
[LT09: Interpreting Normal Distributions](https://lms.lausd.net/page/7707619884)  
[LT10: Interpreting Categorical Data](https://lms.lausd.net/page/7707624044)  
[LT11: Evaluating the Data Gathering Process](https://lms.lausd.net/page/7707625417)

[Go to Top](#top)

## R Programming

### [w3Schools website](https://www.w3schools.com/r/default.asp)

### [w3Schools R compiler](https://www.w3schools.com/r/tryr.asp?filename=demo_compiler)

[Go to Top](#top)

### R Code

[01A Base Frequency Table](https://lms.lausd.net/page/7684930137)  
[01B Base Relative Frequency Table](https://lms.lausd.net/page/7684934619)  
[02 knitr Relative Frequency Table](https://lms.lausd.net/page/7684936179)  
[03 Base Bar Chart](https://lms.lausd.net/page/7684937371)  
[04 ggplot2 Bar Chart](https://lms.lausd.net/page/7684938939)  
[05 Base Pie Chart](https://lms.lausd.net/page/7684939992)  
[06 ggplot2 Pie Chart](https://lms.lausd.net/page/7684943310)

[Go to Top](#top)

## Data Collection and Organization

- **Different types of data:** Data comes in different forms.

  - **Categorical data** represents qualities (e.g., colors, types of fruit).
  - **Numerical data** represents quantities (e.g., height, temperature).
  - **Ordinal data** is categorical data with an order (e.g., rankings, education levels).
  - **Example:** Eye color (categorical), age (numerical), movie ratings (ordinal).

- **Sampling methods:**

  - **Random sampling** ensures every member has an equal chance of being selected.
  - **Stratified sampling** divides the population into groups (strata) and samples from each.
  - **Convenience sampling** uses readily available data (less representative).
  - **Example:** Surveying 100 students randomly vs. surveying the first 100 students in the cafeteria.

- **Data cleaning and manipulation:**

  - **Missing values** need to be addressed.
  - **Outliers** are extreme values that might be errors.
  - **Example:** A survey with some unanswered questions or a recorded height of 10 feet.

- **Basic data structures:**

  - Data is often organized in tables (rows and columns) or spreadsheets.
  - **Rows** represent individuals/observations, and
  - **Columns** represent variables/characteristics.
  - **Example:** A spreadsheet of students' favorite food.

[Go to Top](#top)

## Descriptive Statistics

### **Mean (Average)**

To find the **mean** of a dataset:

1. **Sum all numbers** in the dataset.
2. **Divide by the total count** of numbers.

Mathematically:

$\text{Mean} = \frac{\sum x_i}{n}$

Where:

- $x_i$ represents each value in the dataset.
- $n$ is the total number of values.

**Solution using R:**

```r
numbers <- c(12, 15, 20, 25, 30, 35, 40)
mean_value <- mean(numbers)
print(mean_value)
```

### **Median (Middle Value)**

To find the median:

1. **Sort the values** in ascending order.
2. If $n$ is **odd**, the median is:  
   $\text{Value at position} \left(\frac{n+1}{2}\right)$  
   If $n$ is **even**, the median is the average of the two middle values:  
   $\frac{\text{Value at position } \frac{n}{2} + \text{Value at position } \left(\frac{n}{2} + 1\right)}{2}$

**Solution using R:**

```r
numbers <- c(10, 15, 20, 25, 30, 35, 40)
median_value <- median(numbers)
print(median_value)
```

[Go to Top](#top)

## Math Medic

[Categorical Data and Displays - 10.1](https://cdn.mathmedic.com/image/authenticated/s--bjDVHbF---/v1638558861/Lesson_10_1_Answer_Key_Geometry_Math_Medic_46794688a6.pdf)

- Identify categorical and quantitative variables.
- Organize data in frequency and relative frequency tables.
- Interpret bar charts and pie charts.

[Measures of Center for Quantitative Data - 10.2](https://cdn.mathmedic.com/image/authenticated/s--aqkzOrpk--/v1638558952/Lesson_10_2_Answer_Key_Geometry_Math_Medic_9bd2c5fa4b.pdf)

- Calculate a mean and median from a set of values and from a graph of a distribution.
- Understand the effects of outliers on a mean or median.

[Measures of Spread for Quantitative Data - 10.3](https://cdn.mathmedic.com/image/authenticated/s--w1qYx3B0--/v1643126577/Lesson_10_3_Answer_Key_Geometry_Math_Medic_568fd25a7f.pdf)

- Calculate and interpret range and standard deviation from a data set.
- Use the graph of a set of data to make conclusions about standard deviation.
- Understand the effect of outliers on range and standard deviation.

[Scatterplots and Line of Best Fit - 10.4](https://cdn.mathmedic.com/image/authenticated/s--onBzgD6i--/v1638559060/Lesson_10_4_Answer_Key_Geometry_Math_Medic_1e245adea4.pdf)

- Identify explanatory and response variables.
- Create and describe a scatterplot for two-variable data.
- Interpret the slope and y-intercept of a line of best fit.

[Predictions and Residuals - 10.5](https://cdn.mathmedic.com/image/authenticated/s--t6koVP65--/v1638559312/Lesson_10_5_Answer_Key_Geometry_Math_Medic_8ecac9aecb.pdf)

- Use a line of best fit to make predictions.
- Calculate and interpret a residual using linear models.

[Models for Nonlinear Data - 10.6](https://cdn.mathmedic.com/image/authenticated/s--6LUmR_bC--/v1638559414/Lesson_10_6_Answer_Key_Geometry_Math_Medic_e3f21b9e06.pdf)

- Describe non-linear models.
- Calculate and interpret a residual using non-linear models.

[Go to Top](#top)

## DeltaMath

### **1. Descriptive Statistics and Data Visualization**

1. [Create Frequency Table](https://drive.google.com/file/d/1TTN9-RCTF60hlXividRh66qnLsaPFeub/view?usp=drive_link)
2. [Finding the Mean and the Median](https://drive.google.com/file/d/1yTEsyDeW6_rS4ZL8faOUYpMTuvaOqTiV/view?usp=sharing)
3. [Finding the Mean from a Frequency Table](https://drive.google.com/file/d/1BsymMxvU6kY9qb3AUlC7nw7clJa23NnL/view?usp=drive_link)
4. [Create Histograms](https://drive.google.com/file/d/1SsJr5XtfU5V0vlKnND9E8Y-53DG6LeaA/view?usp=sharing)
5. [Interpret Histograms / Bar Charts](https://drive.google.com/file/d/1_QyjyW4HpPk4XuRn53YjYIUnFZzMzgXp/view?usp=sharing)
6. [Interpret Dot Plot](https://drive.google.com/file/d/1QxQzZtV8T5CoKLjHzLp1jKDeqoJfLi5u/view?usp=drive_link)
7. [Create Box Plot](https://drive.google.com/file/d/13TpqT2R1ioK01EHf3AqSgQFXuf2HcM1J/view?usp=sharing)
8. [Compare Center Visually](https://drive.google.com/file/d/1Qg7sqen1X9_YH449WzjSA24-KEJMXGh7/view?usp=sharing)
9. [Compare Spread Visually](https://drive.google.com/file/d/1WrgiG5h4vMR2MTISeyqOw3WZfb9teSmj/view?usp=sharing)
10. [Calculate Measure of Dispersion](https://drive.google.com/file/d/1o_HsCRjY3ur-5EtA0gZPIwe0dbDN_l7r/view?usp=sharing)
11. [Analyze Datasets](https://drive.google.com/file/d/1OZs_bmkIwi8sd21GdglYWqVoVGYnyJYL/view?usp=sharing)

### **2. Interpreting and Comparing Data Representations**

12. [Interpret Mixed Representations](https://drive.google.com/file/d/1aiS2z-v8Rb7F3ownQ-BwEnjVLI_RuQnR/view?usp=sharing)
13. [Interpreting Calculator Output (Stats)](https://drive.google.com/file/d/13IsJQndt9m2pfcC3jVQ-nvm9zd_Ghbjn/view?usp=sharing)
14. [Interpret Two-Way Tables](https://drive.google.com/file/d/1roLqIG0rhm1WqFRVnBOPNOdlZ9DMOw32/view?usp=sharing)
15. [Percents Two-Way Tables](https://drive.google.com/file/d/1Aec6bbfi88xg_5DkUiK7Mo5Fn_S0ZJXh/view?usp=sharing)
16. [Fill in Values, Two-Way Tables](https://drive.google.com/file/d/1HuFHMzaM9wG7aDEORLLHyRM2hF6aKXwk/view?usp=sharing)

### **3. Scatter Plots, Correlation, and Regression**

17. [Create Scatter Plot from Data Table](https://drive.google.com/file/d/13taX-1jFghrP8X9CEczI-qK88IpyE9R2/view?usp=sharing)
18. [Association/Correlation (Scatter Plot)](https://drive.google.com/file/d/1AXwEdmPxJvNJTcFO7O5_EB9HsFP55-gt/view?usp=sharing)
19. [Interpret Line of Best Fit](https://drive.google.com/file/d/1UK-ozE7Z4CZQ7Ivk5WyuL6HLc4g0ARCH/view?usp=sharing)
20. [Draw Line of Best Fit](https://drive.google.com/file/d/1l06WxQ8tCdzNSdDUO3zfLswHHJN9WqA4/view?usp=sharing)
21. [Prediction from Line of Best Fit](https://drive.google.com/file/d/1AdUWRJuZAXJfmW5kwmR4kLiMLlDgRBWr/view?usp=sharing)
22. [Linear Regressions](https://drive.google.com/file/d/1ZAsnAf_CGhbaNuhdkKVlFPVnN334lmL5/view?usp=sharing)
23. [Exponential Regressions](https://drive.google.com/file/d/1PdsisHdho9cubxgbNhlN-BhHLnHHdmoy/view?usp=sharing)
24. [Correlation Coefficient](https://drive.google.com/file/d/1DVYivPo3KlAPAjL2gNW3VkHuY8IIOgDq/view?usp=sharing)
25. [Strength of Linear Relationships](https://drive.google.com/file/d/1cMg-V7gstgiqzfoOjk32Xa2EtS-Onmfm/view?usp=sharing)
26. [Calculate Residual from Context (Linear)](https://drive.google.com/file/d/19g_encmqihWFNVNa-DMaw6AdRVnd_Vsz/view?usp=sharing)
27. [Linear Regression / Residuals / Best Model](https://drive.google.com/file/d/1Qa0CISywjkN0KWSEJskAYbQlhGTWFR33/view?usp=sharing)

### **4. Probability and Statistical Inference**

28. [Probability with Or](https://drive.google.com/file/d/1IG4splZsPw2Z3a3zJ-rFnfbKmB7Jvd_M/view?usp=sharing)
29. [Probability with And](https://drive.google.com/file/d/1Ktz2W4-FMZ17oQUz3LkGswBZYNbL2NVy/view?usp=sharing)
30. [Probability from a Two Way Table](https://drive.google.com/file/d/1CIAaD_7NNbsnxo_wVn3II89CMZLJw54N/view?usp=sharing)
31. [Conditional Probability from a Table](https://drive.google.com/file/d/1dAyV0Luj5fdmUhfhv1NmjLoiBhpibQ28/view?usp=sharing)
32. [Probability from Verbal Description](https://drive.google.com/file/d/1qlYH2saSzgXUK3gWQj2ygZs9ahrVR_81/view?usp=sharing)
33. [Find Probability Given Probabilities](https://drive.google.com/file/d/1NoYBY1qTx2MyvhPY_AJow3JJ-iH3z63c/view?usp=sharing)
34. [Symbolic Probability Rules](https://drive.google.com/file/d/1VAhvLqD9tusCEaSOkuwZ8TBIbRcoCfi_/view?usp=sharing)
35. [Determine Independence from a Table](https://drive.google.com/file/d/1u-XvCAP1TBn4sdkOItp6AMFPnamJV4D7/view?usp=sharing)

[Go to Top](#top)
