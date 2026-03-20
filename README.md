# Aim

To perform data analysis using the Pandas library in Python by exploring datasets related to student performance and online orders. The objective is to compute frequency distributions, percentage analysis, cross-tabulations, grouping, filtering, and sorting to derive meaningful insights from categorical data.

---

# Theory

## 1. Data Loading and Display
- `pd.read_csv()`  
  Used to load data from a CSV file into a DataFrame.
- `display()`  
  Displays the DataFrame in a structured tabular format.

---

## 2. Frequency Count
- `value_counts()`  
  Returns the count of unique values in a column.  
  Example:
  - Number of students in each grade
  - Number of orders in each category

---

## 3. Percentage Distribution
- `value_counts(normalize=True)`  
  Returns proportions instead of raw counts.
- Multiplying by `100` converts proportions into percentages.

---

## 4. Cross Tabulation
- `pd.crosstab()`  
  Used to compute frequency tables between two categorical variables.
  Examples:
  - Gender vs Grade
  - Department vs Gender
  - Department vs Grade

---

## 5. Normalized Crosstab
- `pd.crosstab(..., normalize='index')`  
  Converts row values into percentages to analyze distribution within categories.

---

## 6. Grouping Data
- `groupby()`  
  Groups data based on a column.
- Combined with `value_counts()` to count occurrences within each group.

---

## 7. Unique Values
- `unique()`  
  Returns all unique values in a column.
- `nunique()`  
  Returns the number of unique values.

---

## 8. Filtering Data
- Boolean indexing (`df[df['Column'] == value]`)  
  Used to extract rows that satisfy a condition.

---

## 9. Sorting Data
- `sort_values(by='Column')`  
  Sorts the DataFrame based on a specified column.

---

## 10. Data Insights Performed

### Student Dataset
- Count of students by grade, gender, and department
- Percentage distribution of grades
- Relationship analysis using cross-tabulation
- Department-wise grade percentage distribution
- Grouped grade counts per department

### Order Dataset
- Category-wise frequency and percentage distribution
- Payment method analysis
- Unique category identification
- Filtering electronics orders
- Sorting orders by category
- Grouping category with payment methods

---

# Conclusion

The experiment demonstrates how Pandas can be effectively used for data analysis and manipulation. Using functions like `value_counts()`, `crosstab()`, `groupby()`, and filtering techniques, we extracted meaningful insights from structured datasets.

In the student dataset, we analyzed academic performance patterns across departments and genders. In the order dataset, we examined customer behavior, category preferences, and payment trends.

Overall, Pandas provides powerful and flexible tools for summarizing, analyzing, and interpreting data efficiently, making it essential for data analysis tasks.
