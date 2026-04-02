# 🚀 Univariate Analysis — Interview Master README

> 🎯 **Goal:** Make you *interview-ready* with deep understanding, not just definitions.

---

# 🧠 1. What is Univariate Analysis?

> "Univariate analysis is the process of analyzing a single variable to understand its distribution, central tendency, spread, and presence of outliers using statistical methods and visualizations."

👉 Keywords interviewer expects:

* Distribution
* Central tendency
* Spread
* Outliers

---

# 📊 2. Types of Data

### Numerical

* Continuous → Age, Salary
* Discrete → Number of students

### Categorical

* Nominal → Gender (no order)
* Ordinal → Ratings (ordered)

👉 Interview trap:

> "Can we use mean on categorical data?"
> ❌ No

---

# 📈 3. Numerical Feature Analysis (Deep Understanding)

## 🔹 Central Tendency

| Measure | Use Case               |
| ------- | ---------------------- |
| Mean    | Normal distribution    |
| Median  | Skewed data / outliers |
| Mode    | Categorical            |

👉 Smart line:

> "Median is more robust to outliers than mean"

---

## 🔹 Spread (Dispersion)

* Range → max - min
* Variance → spread (squared)
* Standard Deviation → actual spread

👉 Interview line:

> "Standard deviation is preferred because it is in the same unit as the data"

---

## 🔹 Shape of Distribution

### Skewness

* Positive → right tail
* Negative → left tail

### Kurtosis

* High → heavy tails (outliers)
* Low → light tails

---

# 📊 4. Categorical Feature Analysis

### Frequency

```python
df['col'].value_counts()
```

### Percentage

```python
df['col'].value_counts(normalize=True)*100
```

👉 Interview tip:

> "Always convert to percentage for better interpretation"

---

# 📉 5. Visualization (What Interviewer Really Wants)

## Numerical

### Histogram

```python
plt.hist(df['Age'])
```

👉 Shows distribution

### KDE Plot

👉 Smooth distribution

### Boxplot

```python
sns.boxplot(x=df['Age'])
```

👉 Detects outliers + spread

---

## Categorical

### Countplot

```python
sns.countplot(x=df['Sex'])
```

---

# 🔥 6. Outliers (Most Asked Topic)

## What are Outliers?

Extreme values far from majority

---

## Detection Methods

### IQR Method

* IQR = Q3 - Q1
* Lower = Q1 - 1.5*IQR
* Upper = Q3 + 1.5*IQR

---

## Interview Answer:

> "I use boxplots and IQR method to detect outliers"

---

# 🚀 7. Real Interview Scenarios

## ❓ Data is highly skewed, what will you do?

✅ Answer:

* Log transformation
* Box-Cox transformation

```python
import numpy as np
df['Age'] = np.log(df['Age'])
```

---

## ❓ Why log transformation?

> "To reduce skewness and stabilize variance"

---

## ❓ When NOT to remove outliers?

> "When they carry important real-world information"

---

# 🧪 8. Coding Round Questions

### ✔ Summary

```python
df.describe()
```

### ✔ Missing Values

```python
df.isnull().sum()
```

### ✔ Distribution Check

```python
sns.histplot(df['Age'], kde=True)
```

---

# ⚡ 9. Rapid Fire (Must Prepare)

* Mean vs Median
* Variance vs Std Dev
* Histogram vs Boxplot
* Skewness types
* Outlier detection methods

---

# 💼 10. Mistakes Most Students Make

❌ Only showing plots, no explanation
❌ Ignoring skewness
❌ Not checking outliers
❌ Using mean blindly

---

# 🎯 11. How to Answer in Interview (Golden Structure)

When asked about a column:

1. Type of data
2. Distribution
3. Skewness
4. Outliers
5. Conclusion

---

# 🔥 Example (Titanic - Age)

> "Age is a numerical variable. It is slightly right-skewed with some outliers. Median is a better measure than mean."

---
