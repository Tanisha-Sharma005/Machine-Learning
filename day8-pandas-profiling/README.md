# 📊 Exploratory Data Analysis (EDA) – Interview Guide

> 🧠 Covers: Bivariate Analysis + Distribution + Pandas Profiling
> 🎯 Goal: Interview Preparation (Concepts + Questions + Answers)

---

## 📌 Overview

This notebook focuses on **Exploratory Data Analysis (EDA)** with emphasis on:

* Distribution Analysis
* Bivariate Analysis
* Feature Relationships
* Automated Profiling

---

## 📊 Key Concepts Covered

### 🔹 1. Distribution Analysis

Understanding how data is spread.

* Histogram
* KDE (Kernel Density Estimation)
* Skewness

---

### 🔹 2. Bivariate Analysis

Analyzing relationship between two variables.

| Type                       | Example            | Plot         |
| -------------------------- | ------------------ | ------------ |
| Numerical vs Numerical     | Age vs Fare        | Scatter Plot |
| Numerical vs Categorical   | Age vs Survived    | Boxplot      |
| Categorical vs Categorical | Gender vs Survived | Countplot    |

---

### 🔹 3. Correlation Analysis

* Measures relationship strength
* Heatmap visualization
* Detects multicollinearity

---

### 🔹 4. Pandas Profiling

* Automated EDA
* Detects:

  * Missing values
  * Correlation
  * Outliers
  * Data types

---

## 🎯 Interview Questions (with Effective Answers)

---

## 🟢 Basic Level

**What is bivariate analysis?**
👉 Analyzes relationship between two variables to find patterns or dependencies.

**Univariate vs Bivariate?**
👉 Univariate = one variable (distribution), Bivariate = two variables (relationship).

**What is correlation?**
👉 Measures strength and direction of linear relationship (-1 to +1).

**What does a scatter plot show?**
👉 Relationship, trend, and outliers between two numerical variables.

**What is a histogram?**
👉 Shows distribution of numerical data using bins.

---

## 🟡 Intermediate Level

**Correlation vs Covariance?**
👉 Covariance shows direction; correlation shows direction + strength (normalized).

**What is KDE and why used?**
👉 Smooth curve to represent distribution; avoids bin dependency.

**What is normalization in histogram?**
👉 Converts counts into density so total area = 1.

**What does `kde=True` do?**
👉 Adds smooth density curve over histogram.

**Boxplot vs Violin plot?**
👉 Boxplot shows summary; violin shows full distribution shape.

---

## 🔴 Advanced Level

**How to handle outliers?**
👉 Detect via plots, treat using IQR/Z-score/capping based on context.

**When is correlation misleading?**
👉 In non-linear relationships, outliers, or hidden variables.

**Pearson vs Spearman?**
👉 Pearson = linear, Spearman = rank-based (robust).

**What is multicollinearity?**
👉 High correlation between features → unstable models.

**How bivariate helps in feature selection?**
👉 Identifies important and redundant features → improves model.

---

## 💡 Code Understanding

```python
sns.histplot(df['Age'], kde=True, stat='density')
```

👉 Histogram + smooth density curve + normalized distribution

---

**Why `annot=True` in heatmap?**
👉 Shows values inside cells.

**Role of `bins`?**
👉 Controls grouping of data.

**Why scatter plot?**
👉 Best for visualizing relationships in numerical data.

**If data is skewed?**
👉 Mean unreliable; prefer median or transformation.

---

🔥 **Interview Line:**

> “I use EDA to understand distributions and relationships before building any model.”

---
