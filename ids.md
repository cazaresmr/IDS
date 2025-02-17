# Introduction to Data Science (Master Notes)

## Top

[IDS Process](#process)

[Mini Project](#mini-project)

[Learning Targets](#learning-targets)

[Desmos](#desmos)

[R Programming](#r-programming)

[Data Collection and Organization](#data-collection-and-organization)

[Data Visualizations](#data-visualizations)

[Descriptive Statistics](#descriptive-statistics)

[Distributions](#distributions)

[Math Medic](#math-medic)

[DeltaMath](#deltamath)

## IDS Process

Here's a **simplified step-by-step process** to analyze a large dataset:

### **1. Understand the Goal**

- What statistical question are we trying to answer?
- What data (key information) do we need?

### **2. Look at the Data**

- Open the dataset and check what’s inside.
- Identify different types of data (numbers (discrete or continuous), categories (nominal or ordinal), dates (formats), etc.).

### **3. Clean the Data**

- Remove empty or duplicate rows.
- Fix any errors (e.g., wrong spellings, incorrect numbers).
- Make sure all data is in the correct format.

### **4. Explore the Data**

- Find basic statistics (average (mean), median (middle value [Q2 first 50% of data]), mode (most frequent value), highest (max), lowest values (min), range (max - min), Q1 (first 25% of data), Q3 (first 75% of data), Interquartile Range [IQR] (Q3 - Q1)), Variance, Standard Deviation (SD or stdev - avearge distance from the mean).
- Make charts (bar graphs, scatter plots, histograms, boxplots, etc.) to see patterns.
- Look for anything unusual (missing values, extreme numbers (outliers)).

### **5. Analyze the Data**

- Compare groups or trends (e.g., Do students who study more get higher grades?).
- Use simple math or formulas to find patterns.
- If needed, test ideas using averages, percentages, or basic equations.

### **6. Explain Your Findings**

- Write a summary of what you discovered.
- Use visualization (charts and graphs) to make it easier to understand.
- Answer the original question clearly.

### **7. Present and Discuss**

- Share your results in a short report or presentation.
- Discuss what the data tells us and what we can learn from it.

[Go to Top](#top)

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

## Desmos

[Desmos File | click to open](https://www.desmos.com/calculator/vqt0e9ejba)

### **1. Entering Data into Desmos**

#### **Step 1: Open a Table**

- Open **Desmos Graphing Calculator** ([https://www.desmos.com/calculator](https://www.desmos.com/calculator)).
- Click the **plus (+) button** and select **Table**.
- Enter your data in columns.

##### **Example: Entering Test Scores and Study Hours**

| Study Hours (\(x\)) | Test Score (\(y\)) |
| ------------------- | ------------------ |
| 2                   | 60                 |
| 3                   | 65                 |
| 5                   | 78                 |
| 6                   | 80                 |
| 8                   | 95                 |
| 9                   | 97                 |

- In **Desmos**, enter:
  ```
  x_1 | y_1
  2   | 60
  3   | 65
  5   | 78
  6   | 80
  8   | 95
  9   | 97
  ```

---

### **2. Creating a Scatter Plot**

Once the table is entered:

- **Desmos automatically plots the points** on the graph.
- You can **zoom in/out** or adjust the window to better see the data.

---

### **3. Finding the Line of Best Fit (Trend Line)**

To see if there’s a relationship between study hours and test scores, use a **linear regression** (best-fit line).

#### **Step 1: Enter the Regression Equation**

In a new Desmos line, type:

```
y_1 ~ m x_1 + b
```

- `m` = slope (rate of change).
- `b` = y-intercept (starting point).
- Desmos will calculate **the best-fit line** and display **the equation**.

#### **Step 2: Interpret the Line**

- If **\( m > 0 \)** (positive slope), test scores **increase** as study hours increase.
- If **\( m \approx 0 \)** (flat line), study hours **do not impact** test scores.

---

### **4. Calculating the Mean, Median, and Standard Deviation**

#### **Step 1: Define the Data as a List**

For test scores:

```
Y = [60, 65, 78, 80, 95, 97]
```

For study hours:

```
X = [2, 3, 5, 6, 8, 9]
```

#### **Step 2: Compute Statistics**

- **Mean (Average)**
  ```
  mean(Y)
  ```
- **Median**
  ```
  median(Y)
  ```
- **Standard Deviation**
  ```
  stdev(Y)
  ```

Desmos will **automatically compute** these values and display them.

---

### **5. Visualizing Data with a Box Plot**

To create a **box plot**, enter:

```
boxplot(Y)
```

- This will show the **minimum, first quartile (Q1), median, third quartile (Q3), and maximum**.

---

### **6. Comparing Two Data Sets**

If you have **two groups** (e.g., students who participate in extracurricular activities vs. those who don’t):

- Define two lists:
  ```
  Group1 = [75, 80, 85, 90, 95]  # Test scores for Group 1
  Group2 = [60, 65, 70, 75, 80]  # Test scores for Group 2
  ```
- Compare means:
  ```
  mean(Group1), mean(Group2)
  ```
- Compare box plots:
  ```
  boxplot(Group1)
  boxplot(Group2)
  ```

✅ **Desmos is great for quick data visualization** like scatter plots, regression lines, and box plots.  
✅ **It helps calculate basic statistics** like mean, median, and standard deviation.  
✅ **Best for small datasets** and simple comparisons.

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

## Data Visualizations

| Graph/Chart Type | Best Used For                                                             | Example Use Case                                                            |
| ---------------- | ------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| **Dot Plot**     | Showing frequency of individual data points, useful for small data sets.  | Displaying the number of students who scored a particular grade on a test.  |
| **Line Plot**    | Tracking changes over time or trends in data.                             | Tracking a student's test scores over multiple semesters.                   |
| **Bar Chart**    | Comparing categories or groups with discrete data.                        | Comparing test scores of different classes.                                 |
| **Pie Chart**    | Showing proportions or percentages of a whole.                            | Showing the percentage of students in different extracurricular activities. |
| **Box Plot**     | Displaying distribution, spread, and outliers in data.                    | Analyzing the spread of test scores and identifying outliers.               |
| **Histogram**    | Showing frequency distributions for large datasets.                       | Displaying the distribution of students’ heights in a school.               |
| **Scatter Plot** | Displaying relationships or correlations between two numerical variables. | Comparing study hours vs. test scores to find a correlation.                |

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

## Distributions

Data distribution shows **how data values are spread out**. It tells us whether values are clustered in one area, evenly spread, or skewed in a certain direction.

### **Example: Test Scores of 100 Students**

| Test Score | Frequency (Number of Students) |
| ---------- | ------------------------------ |
| 50 - 60    | 5                              |
| 60 - 70    | 10                             |
| 70 - 80    | 25                             |
| 80 - 90    | 40                             |
| 90 - 100   | 20                             |

A **histogram** of this data helps us visualize its **distribution**.

---

## **2. Types of Data Distributions**

### **a) Symmetrical Distribution (Normal Distribution)**

📌 **Definition**: A **symmetrical distribution** is one where the left and right sides are mirror images.

📌 **Example**: **Heights of adults**, **IQ scores**, **test scores in a well-designed exam**.

📌 **Characteristics**:  
✅ Bell-shaped curve.  
✅ Mean, median, and mode are equal (or very close).  
✅ Most values are near the center.

📌 **Histogram Example:**

```
      *
    *   *
  *       *
*           *
```

_(Looks like a bell curve!)_

📌 **R Code to Plot a Normal Distribution:**

```r
set.seed(42)  # For reproducibility
data <- rnorm(1000, mean = 75, sd = 10)  # Generate 1000 random numbers with mean 75 and SD 10
hist(data, breaks = 20, main="Normal Distribution", col="lightblue")
```

---

### **b) Asymmetrical Distribution (Skewed Distribution)**

A distribution is **asymmetrical (skewed)** if one side has a longer tail.

#### **i) Right-Skewed (Positively Skewed) Distribution**

📌 **Definition**: A **right-skewed distribution** has a longer tail on the right.

📌 **Example**:  
✅ Salaries (a few people earn very high salaries).  
✅ House prices (most houses are affordable, but some are extremely expensive).

📌 **Characteristics**:

- Mean > Median > Mode (mean is pulled to the right).
- More values are concentrated on the **left** side.

📌 **Histogram Example:**

```
  *
 **
 ***
 ******
 ***********
****************************
```

_(The tail extends to the right.)_

📌 **R Code for Right-Skewed Distribution:**

```r
set.seed(42)
data <- rexp(1000, rate = 0.2)  # Exponential distribution (right-skewed)
hist(data, breaks = 20, main="Right-Skewed Distribution", col="lightgreen")
```

---

#### **ii) Left-Skewed (Negatively Skewed) Distribution**

📌 **Definition**: A **left-skewed distribution** has a longer tail on the left.

📌 **Example**:  
✅ Age of retirement (most retire around 60-65, but some retire early).  
✅ Scores on an easy test (most students score high, few score low).

📌 **Characteristics**:

- Mean < Median < Mode (mean is pulled to the left).
- More values are concentrated on the **right** side.

📌 **Histogram Example:**

```
              *
            **
          ***
     ******
  ***********
****************************
```

_(The tail extends to the left.)_

📌 **R Code for Left-Skewed Distribution:**

```r
set.seed(42)
data <- -rexp(1000, rate = 0.2) + 10  # Transforming an exponential distribution to be left-skewed
hist(data, breaks = 20, main="Left-Skewed Distribution", col="salmon")
```

---

## **3. Uniform and Bimodal Distributions**

### **a) Uniform Distribution**

📌 **Definition**: **All values occur with equal probability**.

📌 **Example**:  
✅ Rolling a fair die (1, 2, 3, 4, 5, 6 all have equal chances).  
✅ Assigning random numbers to students in a class.

📌 **Histogram Example:**

```
********
********
********
********
********
********
```

_(Bars are of equal height.)_

📌 **R Code for Uniform Distribution:**

```r
set.seed(42)
data <- runif(1000, min=1, max=10)  # Random numbers between 1 and 10
hist(data, breaks = 10, main="Uniform Distribution", col="orange")
```

---

### **b) Bimodal Distribution**

📌 **Definition**: **Two peaks in the data** (data comes from two different groups).

📌 **Example**:  
✅ Exam scores of two different classes.  
✅ Heights of men and women in a population.

📌 **Histogram Example:**

```
   *
  ***
 *****
  ***
   *
  ***
 *****
  ***
   *
```

_(Two peaks appear in the graph.)_

📌 **R Code for Bimodal Distribution:**

```r
set.seed(42)
data1 <- rnorm(500, mean = 60, sd = 5)
data2 <- rnorm(500, mean = 80, sd = 5)
data <- c(data1, data2)  # Combine two normal distributions
hist(data, breaks = 20, main="Bimodal Distribution", col="purple")
```

---

## **4. Why Does Data Distribution Matter?**

1️⃣ **Tells us about the shape of the data** (helps in making predictions).  
2️⃣ **Affects statistical analysis** (e.g., mean and median behave differently in skewed distributions).  
3️⃣ **Used in decision-making** (e.g., setting salary levels, analyzing test scores).

---

## **5. Real-World Applications**

| **Field**       | **Example**                  | **Type of Distribution** |
| --------------- | ---------------------------- | ------------------------ |
| Finance         | Income levels in a country   | Right-skewed             |
| Education       | Test scores in a fair exam   | Normal (Bell Curve)      |
| Gaming          | Rolling a fair die           | Uniform                  |
| Medical Studies | Blood pressure of patients   | Normal                   |
| Marketing       | Customer spending habits     | Right-skewed             |
| Social Science  | Population ages in a country | Left-skewed              |

✅ **Symmetrical distribution**: Normal (bell-shaped).  
✅ **Asymmetrical distribution**: Skewed left or right.  
✅ **Uniform distribution**: All values occur equally.  
✅ **Bimodal distribution**: Two peaks, indicating two groups.  
✅ **Distributions help in decision-making, data analysis, and real-world problem-solving.**

[Go to Top](#top)

## Mini Project

Content for the mini project section.

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

## Mini-Project: Analyzing Student Performance Using R

### **Objective**

In this mini-project, we will analyze a dataset containing students' study hours, test scores, and participation in extracurricular activities. Our goal is to determine:

1. Whether studying more leads to higher test scores.
2. Whether students who participate in extracurricular activities perform better.

---

## **Step 1: Creating the Dataset**

First, we will create a dataset using **R vectors** and convert it into a **data frame**.

````r
# Create vectors for each column
Student <- paste("Student", 1:100, sep="_")  # Generate 100 student names
set.seed(42)  # Ensure reproducibility

# Generate random study hours (between 1 and 10)
Study_Hours <- sample(1:10, 100, replace = TRUE)

# Generate test scores based on study hours with some randomness
Test_Score <- pmin(100, pmax(50, 50 + Study_Hours * 5 + rnorm(100, 0, 10))) # Scores between 50-100

# Round test scores to the nearest whole number (percent)
Test_Score <- round(Test_Score)

# Generate random extracurricular participation (Yes or No)
Extracurricular <- sample(c("Yes", "No"), 100, replace = TRUE, prob = c(0.5, 0.5))

# Create a data frame
df <- data.frame(Student, Study_Hours, Test_Score, Extracurricular)

# View the first few rows
head(df)
```

---

## **Step 2: Saving the Dataset**

To save and reuse the dataset, we can export it as a **CSV file**.

```r
write.csv(df, "student_performance.csv", row.names = FALSE)
````

---

## **Step 3: Load and Inspect the Dataset**

If you’ve already saved the dataset, you can load it again with:

```r
data <- read.csv("student_performance.csv")

# View first few rows
head(data)

# Check column names
colnames(data)
```

---

## **Step 4: Basic Data Exploration**

### **1. Summary Statistics**

```r
summary(data)  # Provides a quick summary of the dataset
```

### **2. Check for Missing Values**

```r
sum(is.na(df))  # Returns total number of missing values
```

---

## **Step 5: Data Analysis**

### **1. Find Average Study Hours and Test Scores**

```r
mean(data$Study_Hours, na.rm = TRUE)  # Average study hours
mean(data$Test_Score, na.rm = TRUE)   # Average test score
```

---

### **2. Relationship Between Study Hours and Test Scores**

#### **Scatter Plot**

```r
plot(df$Study_Hours, df$Test_Score,
     main="Study Hours vs Test Score",
     xlab="Study Hours", ylab="Test Score",
     col="blue", pch=19)

# Add a trend line (linear regression)
abline(lm(Test_Score ~ Study_Hours, data=df), col="red")
```

#### **Correlation Between Study Hours and Test Scores**

```r
cor(df$Study_Hours, df$Test_Score, use = "complete.obs")
```

- A correlation **close to 1** suggests a strong positive relationship.
- A correlation **close to 0** means no relationship.

---

### **3. Compare Test Scores Based on Extracurricular Participation**

#### **Box Plot**

```r
boxplot(Test_Score ~ Extracurricular, data=df,
        main="Test Scores by Extracurricular Participation",
        xlab="Extracurricular", ylab="Test Score",
        col=c("lightblue", "lightgreen"))
```

- If one group has **higher scores** on average, participation might influence performance.

---

### **4. Statistical Test: Do Students in Extracurricular Activities Perform Better?**

A **t-test** compares the average test scores of students who participate in extracurricular activities vs. those who do not.

```r
t.test(Test_Score ~ Extracurricular, data=df)
```

- **p-value < 0.05** → Significant difference (extracurriculars may impact performance).
- **p-value > 0.05** → No significant difference.

---

## **Step 6: Summary and Interpretation**

1. **Does more studying lead to higher scores?**

   - Check the **correlation** and **scatter plot**.
   - If there’s a strong positive trend, studying more likely improves scores.

2. **Do students in extracurricular activities perform better?**

   - Look at the **box plot** and **t-test results**.
   - If scores are significantly different, extracurricular activities may impact performance.

3. **Discussion:**
   - What other factors could influence test scores? (e.g., sleep, tutoring, school resources)
   - Would a larger dataset change the findings?

---

### **Final Notes for Beginners**

- **Why are we using summary statistics?** To understand general trends.
- **Why are we using a scatter plot?** To visually see if there's a relationship.
- **Why do we use a t-test?** To compare two groups statistically.

<hr>

✅ **How the numbers are distributed:**

- Around **68%** of the numbers fall within **one standard deviation** of the mean (65–85).
- Around **95%** of the numbers fall within **two standard deviations** (55–95).

### **Summary of What This Code Does**

1️⃣ **Ensures reproducibility** (`set.seed(42)`).  
2️⃣ **Generates random numbers** that follow a **normal distribution** (`rnorm(1000, mean = 75, sd = 10)`).  
3️⃣ **Visualizes the distribution** using a **histogram** (`hist(data, breaks = 20, col="lightblue")`).

---

### **Interpreting the T-Test Results**

The t-test is used to check if there is a **significant difference** in **test scores** between students who participate in **extracurricular activities** ("Yes") and those who do not ("No").

---

### **Key Results:**

#### **1. Mean Scores for Each Group**

- **Students without extracurricular activities ("No")**: **75.02**
- **Students with extracurricular activities ("Yes")**: **77.15**
- **Difference**: **77.15 - 75.02 = 2.13** (small difference)

#### **2. T-test Statistics**

- **t = -0.70588** → The test statistic measures the difference between groups in terms of standard error.
- **df = 90.59** → Degrees of freedom for the test.
- **p-value = 0.4821** → This tells us **if the difference is statistically significant**.

#### **3. Confidence Interval (95%)**

- **Range: [-8.14, 3.87]**
- Since **zero** is included in this range, it means that the difference in means could be **zero** (no real difference).

---

### **Final Conclusion:**

❌ **There is NO significant difference in test scores based on extracurricular participation.**

- The **p-value (0.4821) is greater than 0.05**, meaning the difference is **not statistically significant**.
- The **confidence interval includes zero**, suggesting that **the true difference could be zero**.

✅ **What This Means in Simple Terms:**

- Students who participate in extracurricular activities **do not score significantly higher or lower** than those who don’t.
- The difference in test scores (2.13 points) could have occurred **by chance** rather than due to extracurricular activities.
