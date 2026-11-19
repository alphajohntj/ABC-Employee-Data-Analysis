# ABC Company Employee Data Analysis

## 1. Project Overview

This project focuses on analyzing employee data from ABC Company using Python. The dataset contains information about 458 employees across different teams and job positions.

The main objective is to preprocess the dataset, perform exploratory data analysis (EDA), identify meaningful patterns, and present the findings through graphical visualizations.

The analysis helps understand employee distribution, age demographics, team structure, salary expenditure, and the relationship between employee age and salary.

## 2. Dataset Description

The dataset contains **458 rows and 9 columns**.

The columns include:

- **Name:** Employee name.
- **Team:** Team to which the employee belongs.
- **Number:** Employee jersey or identification number.
- **Position:** Employee's playing position.
- **Age:** Employee's age.
- **Height:** Employee's height.
- **Weight:** Employee's weight.
- **College:** College attended by the employee.
- **Salary:** Employee's salary.

The dataset was provided for the ABC Company employee analysis project.

## 3. Technologies and Libraries Used

The following Python libraries were used:

- **Pandas:** Data loading, cleaning, grouping, and analysis.
- **NumPy:** Generating random height values and numerical operations.
- **Matplotlib:** Creating charts and graphical representations.
- **Seaborn:** Creating statistical visualizations, including scatter plots and regression plots.

## 4. Data Preprocessing

The following preprocessing steps were performed:

### 4.1 Importing Libraries

Imported Pandas, NumPy, Matplotlib, and Seaborn for data manipulation, analysis, and visualization.

### 4.2 Loading the Dataset

Loaded the CSV file into a Pandas DataFrame using `pd.read_csv()`.

### 4.3 Understanding the Dataset

Used functions such as:

- `head()` to view the first few records.
- `info()` to understand column data types and non-null values.
- `shape` to check the number of rows and columns.
- `isnull().sum()` to identify missing values.

### 4.4 Correcting the Height Column

The original Height column contained incorrect data. It was replaced with randomly generated integer values between **150 and 180**, inclusive, using NumPy.

A random seed was used to make the generated values reproducible.

### 4.5 Saving the Cleaned Dataset

The preprocessed dataset was saved as:

`preprocessed_abc_company_employees.csv`

The dataset retains its original 458 rows and 9 columns.

## 5. Data Analysis and Graphical Representations

The following analysis tasks were completed.

### 5.1 Employee Distribution Across Teams

Calculated the number and percentage of employees in each team using Pandas.

**Graphical representations:**
- Bar chart showing the number of employees in each team.
- Pie chart showing the percentage distribution of employees across teams.

**Insight:** The analysis provides an overview of how employees are distributed across the company's 30 teams and helps identify teams with higher or lower employee counts.

### 5.2 Employee Segregation by Position

Grouped employees according to their positions and calculated the count and percentage for each position.

**Graphical representations:**
- Bar chart showing employee count by position.
- Pie chart showing the percentage distribution by position.

**Insight:** Shooting Guards (SG) have the highest employee count, with 102 employees (22.27%). Centers (C) have the lowest count, with 79 employees (17.25%).

### 5.3 Predominant Age Group

Created age groups using Pandas `cut()`:

- 18–25
- 26–30
- 31–35
- 36–40

Calculated the number and percentage of employees in each age group.

**Graphical representations:**
- Bar chart showing employee distribution by age group.
- Pie chart showing the percentage distribution by age group.

**Insight:** The 18–25 age group is the predominant group, with 200 employees, representing approximately 43.67% of the workforce.

### 5.4 Salary Expenditure by Team and Position

Used Pandas `groupby()` and `sum()` to calculate total salary expenditure for each team and position.

**Graphical representations:**
- Bar chart showing total salary expenditure by team.
- Bar chart showing total salary expenditure by position.

**Insights:**
- Cleveland Cavaliers have the highest salary expenditure by team, amounting to 106,988,689.
- Center (C) has the highest salary expenditure by position, amounting to 466,377,332.

These findings show that salary expenditure depends not only on employee count but also on individual salary amounts.

### 5.5 Correlation Between Age and Salary

Calculated the Pearson correlation coefficient between Age and Salary using Pandas.

**Graphical representations:**
- Scatter plot showing the relationship between employee age and salary.
- Regression plot with a trend line to visualize the overall relationship.

**Insight:** The correlation coefficient is approximately **0.214**, indicating a weak positive relationship between age and salary. This suggests that salary tends to increase slightly with age, but the relationship is not strong.

## 6. Summary of Key Findings

| Analysis | Key Finding |
|---|---|
| Total Employees | 458 |
| Total Teams | 30 |
| Total Positions | 5 |
| Highest Employee Count by Position | SG – 102 employees |
| Lowest Employee Count by Position | C – 79 employees |
| Predominant Age Group | 18–25 – 200 employees |
| Highest Salary by Team | Cleveland Cavaliers |
| Highest Salary by Position | Center (C) |
| Age-Salary Correlation | 0.214 (Weak Positive) |

## 7. Conclusion

This project demonstrates how Python can be used to clean, analyze, and visualize employee data effectively.

The analysis reveals that the 18–25 age group represents the largest portion of the workforce, Shooting Guards are the most common position, and Cleveland Cavaliers have the highest total salary expenditure among teams.

The Center position has the highest total salary expenditure despite having the lowest employee count among the five positions. The correlation analysis also indicates a weak positive relationship between age and salary.

Overall, the project provides useful insights into employee demographics, team distribution, and salary patterns. These findings demonstrate how data analysis and visualization can support better understanding and data-driven decision-making.

## 8. Limitations and Additional Information

- The Height column was replaced with randomly generated values between 150 and 180 as required by the project instructions. These values should not be treated as actual employee heights.
- The dataset contains missing values in some columns.
- Salary expenditure calculations exclude records with missing salary values. There are 11 such records.
- Correlation indicates association, not causation.
- The analysis is based only on the information available in the provided dataset.

## 9. Project Files

The project folder contains:

- `abc_company_employees.csv` – Original dataset.
- `preprocessed_abc_company_employees.csv` – Preprocessed dataset.
- `README.md` – Project documentation.
- `ABC_Company_Employee_Analysis.ipynb` – Jupyter Notebook containing the analysis and visualizations (if included).

## 10. How to Run the Project

### Step 1: Install Required Libraries

```bash
python -m pip install pandas numpy matplotlib seaborn jupyter
```

### Step 2: Open the Project Folder

Open the project folder in Cursor IDE or another Python editor.

### Step 3: Run the Python File

ABC_Company_Employee_Analysis.ipynb

### Step 4: View the Results

The program displays analysis results and graphical visualizations. The cleaned dataset is saved as a CSV file.

---

**Project:** ABC Company Employee Data Analysis

**Language:** Python

**Tools:** Pandas, NumPy, Matplotlib, Seaborn

**Project Type:** Data Cleaning, Exploratory Data Analysis (EDA), and Data Visualization