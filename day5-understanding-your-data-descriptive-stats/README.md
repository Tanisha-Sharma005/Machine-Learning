# 📊 Descriptive Statistics (Understanding Your Data) — Interview README

This README is designed to help you prepare for **Data Science / Machine Learning interviews** based on the notebook: **"Understanding Your Data - Descriptive Statistics"**.

It covers **Basic → Intermediate → Advanced** questions along with short explanations.

---

# 🧠 1. Basic Interview Questions

### ❓ What is Descriptive Statistics?

Descriptive statistics summarize and describe the main features of a dataset using numbers and visualizations.

---

### ❓ What are the types of Descriptive Statistics?

1. Measures of Central Tendency
2. Measures of Dispersion
3. Measures of Shape

---

### ❓ What is Mean?

Average of all values.

👉 Formula:
Sum of values / Total number of values

---

### ❓ What is Median?

Middle value after sorting data.

---

### ❓ What is Mode?

Most frequently occurring value.

---

### ❓ What is Range?

Difference between max and min value.

---

# 📈 2. Intermediate Questions

### ❓ What is Variance?

Measures how far data points spread from the mean.

---

### ❓ What is Standard Deviation?

Square root of variance.

👉 It tells how much data deviates from the mean.

---

### ❓ Difference between Variance and Standard Deviation?

* Variance → squared units
* Standard deviation → original units (more interpretable)

---

### ❓ What is IQR (Interquartile Range)?

IQR = Q3 - Q1

👉 Used to detect outliers

---

### ❓ What are Quartiles?

* Q1 → 25%
* Q2 → Median (50%)
* Q3 → 75%

---

### ❓ What is Skewness?

Measures asymmetry of data.

* Positive skew → tail on right
* Negative skew → tail on left

---

### ❓ What is Kurtosis?

Measures "tailedness" of distribution.

* High kurtosis → more outliers
* Low kurtosis → fewer outliers

---

# 📊 3. Practical / Pandas-Based Questions

### ❓ What does `df.describe()` do?

Provides summary statistics like:

* mean
* std
* min
* max
* quartiles

---

### ❓ Why use `np.round(xtrain.describe(),1)`?

Rounds output to **1 decimal place** for readability.

---

### ❓ How to check missing values?

```python
df.isnull().sum()
```

---

### ❓ How to find correlation?

```python
df.corr()
```

---

### ❓ What is correlation?

Measures relationship between variables.

Range: -1 to +1

---

### ❓ Difference between Covariance and Correlation?

* Covariance → direction only
* Correlation → direction + strength (normalized)

---

# 📉 4. Visualization-Based Questions

### ❓ What is Histogram?

Shows distribution of data.

---

### ❓ What is Boxplot?

Used to detect outliers and visualize spread.

---

### ❓ What is Scatter Plot?

Shows relationship between two variables.

---

# 🚀 5. Advanced Interview Questions

### ❓ How do you detect outliers?

1. IQR method
2. Z-score method

---

### ❓ What is Z-score?

Measures how many standard deviations a value is from the mean.

---

### ❓ Why is Standardization important?

* Required for ML algorithms (e.g., Logistic Regression, SVM)
* Helps features scale equally

---

### ❓ Difference between Normalization and Standardization?

* Normalization → scales between 0 and 1
* Standardization → mean = 0, std = 1

---

### ❓ What is Data Distribution?

Pattern of data values (normal, skewed, uniform, etc.)

---

# 💡 6. Scenario-Based Questions

### ❓ When should you use Median instead of Mean?

👉 When data has **outliers**

---

### ❓ When is Standard Deviation not reliable?

👉 When data is highly skewed

---

### ❓ Why is EDA important before ML?

* Understand data
* Detect issues
* Improve model performance

---

# 🧪 7. Coding Questions (Important for Interviews)

### ✔ Calculate Mean

```python
import numpy as np
np.mean(data)
```

---

### ✔ Calculate Standard Deviation

```python
np.std(data)
```

---

### ✔ Plot Histogram

```python
import matplotlib.pyplot as plt
plt.hist(data)
plt.show()
```

---

### ✔ Boxplot

```python
plt.boxplot(data)
```
