# Introduction to Data Science

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

## DeltaMath

Topics below

## R Programming

### [w3Schools website](https://www.w3schools.com/r/default.asp)

### [w3Schools R compiler](https://www.w3schools.com/r/tryr.asp?filename=demo_compiler)

### R code

[01A Base Frequency Table](https://lms.lausd.net/page/7684930137)

[01B Base Relative Frequency Table](https://lms.lausd.net/page/7684934619)

[02 knitr Relative Frequency Table](https://lms.lausd.net/page/7684936179)

[03 Base Bar Chart](https://lms.lausd.net/page/7684937371)

[04 ggplot2 Bar Chart](https://lms.lausd.net/page/7684938939)

[05 Base Pie Chart](https://lms.lausd.net/page/7684939992)

[06 ggplot2 Pie Chart](https://lms.lausd.net/page/7684943310)

## Data Collection and Organization

- Different types of data: Data comes in different forms.
- Categorical data represents qualities (e.g., colors, types of fruit).
- Numerical data represents quantities (e.g., height, temperature).
- Ordinal data is categorical data with an order (e.g., rankings, education levels).
- Example: Eye color (categorical), age (numerical), movie ratings (ordinal).
- Sampling methods: We often study a sample of a population. Random sampling ensures every member has an equal chance of being selected.
- Stratified sampling divides the population into groups (strata) and samples from each.
- Convenience sampling uses readily available data (less representative).
- Example: Surveying 100 students randomly vs. surveying the first 100 students in the cafeteria.
- Data cleaning and manipulation: Real-world data is messy.
- Missing values need to be addressed.
- Outliers are extreme values that might be errors.
- Example: A survey with some unanswered questions or a recorded height of 10 feet.
- Basic data structures:
- Data is often organized in tables (rows and columns) or spreadsheets.
- Rows represent individuals/observations, and
- Columns represent variables/characteristics.
- Example: A spreadsheet of students' favorite food

## Descriptive Statistics

Calculating central tendency measures:

### Mean is the average.

To find the **mean** (average) of a large set of numbers, follow these steps:

1.  **Sum all the numbers** in the dataset.
2.  **Divide the sum by the total count** of numbers.

Mathematically, the mean is given by:

$\text{Mean} = \frac{\sum x_i}{n}$

Where:

- $x_i$ represents each value in the dataset.
- $n$ is the total number of values.

### **Solution using R:**

```r
# Define the dataset
numbers <- c(12, 15, 20, 25, 30, 35, 40)

# Calculate the mean
mean_value <- mean(numbers)

# Print the result
print(mean_value)

```

### Median is the middle value.

To find the median of a large set of values, you can follow these steps:

1.  **Sort the values** in ascending order.
2.  **Determine the median:** - If the number of values (**n**) is **odd**, the median is the middle value:  
     $\text{ Value at position: } \left(\frac{n+1}{2}\right)$ - If **n** is **even**, the median is the average of the two middle values:
    $\frac{\text{Value at position } \frac{n}{2} + \text{Value at position } \left(\frac{n}{2} + 1\right)}{2}$

### **Solution using R:**

```r
# Define the dataset
numbers <- c(10, 15, 20, 25, 30, 35, 40)

# Calculate the median
median_value <- median(numbers)

# Print the result
print(median_value)

```

### Mode is the most frequent value

The **mode** is the number that appears most frequently in a dataset. Here's how to find it:

1.  **Count the frequency** of each value.
2.  **Identify the value(s) with the highest frequency**:
    - If one number appears most often, it's the **single mode**.
    - If multiple numbers have the same highest frequency, the dataset is **multimodal**.
    - If all values appear with the same frequency, the dataset has **no mode**.

---

### **Example Problem:**

Find the mode of the dataset:

4,1,2,2,3,4,4,5,6,4,2,24, 1, 2, 2, 3, 4, 4, 5, 6, 4, 2, 2

### **Solution using R:**

```r
# Define the dataset
numbers <- c(4, 1, 2, 2, 3, 4, 4, 5, 6, 4, 2, 2)

# Create a table of frequencies
freq_table <- table(numbers)

# Find the value(s) with the highest frequency
mode_value <- as.numeric(names(freq_table)[freq_table == max(freq_table)])

# Print the result
print(mode_value)
```

### **Expected Output:**

```
4 2
```

**Explanation:** The numbers **4** and **2** both appear **4 times**, so this dataset is **bimodal**.

### Understanding variability:

### Range is the difference between the highest and lowest values.

### **How to Find the Range**

The **range** of a dataset is the difference between the **maximum** and **minimum** values.

### **Formula:**

$\text{Range} = \text{Max value} - \text{Min value}$

### **Example Problem:**

Find the range of the dataset:

$8,14,22,35,418, 14, 22, 35, 41$

### **Solution Using R:**

```r
# Define the dataset
numbers <- c(8, 14, 22, 35, 41)

# Calculate the range
range_value <- max(numbers) - min(numbers)

# Print the result
print(range_value)
```

### **Output:**

```
33
```

### Standard deviation measures how spread out the data is from the mean.

### **How to Find the Standard Deviation**

The **standard deviation (SD)** measures the spread of a dataset relative to its mean. A lower SD indicates values are close to the mean, while a higher SD indicates more variability.

#### **Formula for Population Standard Deviation:**

$\sigma = \sqrt{\frac{\sum (x_i - \bar{x})^2}{n}}$

Where:

- $σ$ = population standard deviation
- ∑ = **Summation symbol** (sum of all values)
- $x_i$ = each data value
- $\bar{x}$ = mean of the data
- $n$ = number of values

For **sample standard deviation**, use n−1n-1 in the denominator:

#### **Formula for Sample Standard Deviation:**

$\text{s} = \sqrt{\frac{\sum (x_i - \bar{x})^2}{n-1}}$

$s$ = sample standard deviation

---

### **Example Problem:**

Find the standard deviation for the dataset:

$10,15,20,25,30,35,40$

#### **Solution Using R:**

```r
# Define the dataset
numbers <- c(10, 15, 20, 25, 30, 35, 40)

# Calculate the standard deviation (sample SD)
sd_value <- sd(numbers)

# Print the result
print(sd_value)
```

#### **Output:**

```
11.18034
```

### Creating visualizations:

### Bar charts show categorical data.

```r
# We need this line of code to show graphs in w3Schools compiler
bitmap(file="out.png")

# Create categorical data
grades <- c("A", "B", "C", "D", "F")  # Categories
students <- c(10, 15, 20, 5, 3)        # Frequency of each category

# Create bar plot
barplot(students,
        names.arg = grades,
        col = "blue",
        main = "Student Grades Distribution",
        xlab = "Grades",
        ylab = "Number of Students")
```

### Histograms show the distribution of numerical data.

```r
# We need this line of code to show graphs in our compiler
bitmap(file="out.png")

# Create numerical data (test scores)
test_scores <- c(45, 50, 55, 60, 65, 70, 72, 74, 78, 80,
                 82, 85, 87, 90, 92, 95, 98, 100)

# Create histogram
hist(test_scores,
     col = "blue",
     main = "Distribution of Test Scores",
     xlab = "Scores",
     ylab = "Frequency",
     breaks = 5,  # Number of bins
     border = "black")
```

### Scatter plots show the relationship between two numerical variables.

```r
# We need this line of code to show graphs in our compiler
bitmap(file="out.png")

# Create numerical data
study_hours <- c(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
exam_scores <- c(50, 55, 65, 70, 75, 80, 85, 88, 92, 95)

# Create scatter plot
plot(study_hours, exam_scores,
     main = "Study Hours vs Exam Scores",
     xlab = "Study Hours",
     ylab = "Exam Score",
     col = "blue",
     pch = 16)  # pch = 16 makes solid circles

# Optionally, add a trend line
abline(lm(exam_scores ~ study_hours), col = "red", lwd = 2)
```

### Examples: A bar chart of favorite colors, a histogram of student heights, a scatter plot of study time vs. test scores.

## Inferential Statistics

### Basic probability concepts:

- Independent events don't affect each other (e.g., flipping a coin twice).
- Conditional probability is the probability of an event given another event has occurred.
- Examples: The probability of rolling a 6 on a die (independent), the probability of rain given cloudy skies (conditional).

## Data Analysis and Interpretation

- Identifying patterns and relationships: Look for trends, correlations, and clusters in data.
- Example: Sales increase during the holiday season.
- Correlation vs. causation: Correlation means two variables are related.
- Causation means one variable causes the other.
- Correlation doesn't imply causation!
- Example: Ice cream sales and crime rates might be correlated (both increase in summer), but ice cream doesn't cause crime.
- Recognizing bias: Bias can occur in data collection (e.g., asking leading questions) or analysis (e.g., cherry-picking data).
- Example: A survey about political opinions that only samples people from one political party.

## Basic Programming Skills

- Introduction to R: R is a powerful language for data analysis. We can use it to perform statistical calculations, create visualizations, and manipulate data.
- Example: mean(student_ages) would calculate the average age of students if we had a list of ages called student_ages in R.
- Basic data manipulation and visualization commands:
- R has functions for sorting, filtering, and summarizing data.
- It also has packages for creating various types of plots.
- Example: ggplot(data, aes(x = age, y = height)) + geom_point() would create a scatter plot of age vs. height.

## Real-world Applications

- Designing simple data-driven projects: Come up with a question, collect data, analyze it, and draw conclusions. Example: "Does the amount of sleep a student gets correlate with their test scores?"

<hr>

<!-- [Create Frequency Table](https://drive.google.com/file/d/1TTN9-RCTF60hlXividRh66qnLsaPFeub/view?usp=drive_link) -->

<a href="https://drive.google.com/file/d/1TTN9-RCTF60hlXividRh66qnLsaPFeub/view?usp=drive_link" target="_blank">Create Frequency Table</a>

[Finding the Mean from a Frequency Table](https://drive.google.com/file/d/1BsymMxvU6kY9qb3AUlC7nw7clJa23NnL/view?usp=drive_link)

[Interpret Dot Plot](https://drive.google.com/file/d/1QxQzZtV8T5CoKLjHzLp1jKDeqoJfLi5u/view?usp=drive_link)

[Interpret Histograms / Bar Charts](#)

[Create Histograms](#)

[Interpret Box Plot](#)

[Create Box Plot](#)

[Compare Center Visually](#)

[Compare Spread Visually](#)

[Interpret Mixed Representations](#)

[Interpreting Calculator Output (Stats)](#)

[Interpret Two-Way Tables]()

[Percents Two-Way Tables]()

[Create Scatter Plot from Data Table]()

[Association/Correlation (Scatter Plot)]()

[Interpret Line of Best Fit]()

[Draw Line of Best Fit]()

[Linear Regressions]()

[Exponential Regressions]()

[Correlation Coefficient]()

[Strength of Linear Relationships]()

[Calculate Residual from Context (Linear)]()

[Linear Regression / Residuals / Best Model]()

[Probability with Or]()

[Probability with And]()

[Probability from a Two Way Table]()

[Conditional Probability from a Table]()

[Probability from Verbal Description]()

[Find Probability Given Probabilities]()

[Symbolic Probability Rules]()

[Determine Independence from a Table]()
