# 📊 Bivariate Analysis – Interview Questions

---

# 🎯 Interview Questions (Basic → Advanced)

---

## 🟢 Basic Level

### 1. What is bivariate analysis?

👉 Bivariate analysis studies the **relationship between two variables** to identify patterns, trends, or dependencies.

---

### 2. Difference between univariate and bivariate analysis?

👉 Univariate analyzes **one variable (distribution)**, while bivariate analyzes **relationship between two variables**.

---

### 3. What is correlation?

👉 Correlation measures the **strength and direction of a linear relationship** between two variables, ranging from **-1 to +1**.

---

### 4. What does a scatter plot show?

👉 It shows:

* Relationship between two numerical variables
* Trend (positive/negative)
* Outliers and clusters

---

### 5. What is a histogram?

👉 A histogram shows the **distribution of a numerical variable** by grouping data into bins.

---

## 🟡 Intermediate Level

---

### 6. Difference between correlation and covariance?

👉

* **Covariance** shows direction of relationship (positive/negative)
* **Correlation** shows both direction + strength (scaled between -1 and 1)

✔ Correlation is normalized version of covariance.

---

### 7. What is KDE and why is it used?

👉 KDE (Kernel Density Estimation) is a **smooth curve** representing data distribution.

✔ Used because:

* Removes bin dependency
* Gives continuous distribution
* Easier to interpret than histogram

---

### 8. What is normalization in histogram?

👉 Normalization converts counts into **probability density** such that:

✔ Total area under histogram = 1

👉 Done using:

```python
stat='density'
```

---

### 9. What does `kde=True` do in seaborn?

👉 It adds a **smooth density curve** over the histogram to better visualize distribution.

---

### 10. Difference between boxplot and violin plot?

👉

* **Boxplot** → shows summary (median, quartiles, outliers)
* **Violin plot** → shows full distribution shape + density

✔ Violin = Boxplot + KDE

---

## 🔴 Advanced Level

---

### 11. How do you handle outliers in bivariate analysis?

👉

* Detect using boxplot/scatter plot
* Handle using:

  * IQR method
  * Z-score
  * Capping or transformation

✔ Always analyze before removing.

---

### 12. When can correlation be misleading?

👉

* Non-linear relationships
* Presence of outliers
* Hidden/confounding variables

✔ Example: quadratic relationship → correlation may be near 0

---

### 13. Difference between Pearson and Spearman correlation?

👉

* **Pearson** → measures linear relationship (sensitive to outliers)
* **Spearman** → measures rank/monotonic relationship (robust)

---

### 14. What is multicollinearity?

👉 When independent variables are **highly correlated with each other**.

✔ Problems:

* Unstable model coefficients
* Difficult interpretation

---

### 15. How does bivariate analysis help in feature selection?

👉

* Identifies strong relationships with target
* Removes irrelevant features
* Detects redundancy (multicollinearity)

✔ Improves model performance

---

## 💡 Code Understanding Questions

---

### 16. What does this line do?

```python
sns.histplot(df['Age'], kde=True, stat='density')
```

👉

* Plots histogram of Age
* `kde=True` → adds smooth density curve
* `stat='density'` → normalizes area to 1

---

### 17. Why do we use `annot=True` in heatmap?

👉 It displays **numerical values inside the heatmap cells** for better readability.

---

### 18. What is the use of `bins` in histogram?

👉 Controls how data is grouped.

✔ Too few bins → loss of detail
✔ Too many bins → noisy plot

---

### 19. Why scatter plot is preferred for numerical variables?

👉 Because it clearly shows:

* Relationship
* Trend
* Outliers
* Pattern (linear/non-linear)

---

### 20. What happens if data is highly skewed?

👉

* Mean becomes unreliable
* Median is preferred
* Distribution becomes asymmetric

✔ May require transformation (log, scaling)

---

# 🚀 Final Tip (Must Say in Interview)

👉 “I first visualize relationships using plots like scatter/boxplot, then validate them using statistical measures like correlation.”

---
