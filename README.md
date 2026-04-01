# 🤖 Machine Learning Complete Handbook

> 🚀 Concepts + Code + Interview Questions (Basic → Advanced)

---

## 📌 What is Machine Learning?

Machine Learning is a technique where computers learn patterns from data and make predictions without being explicitly programmed.

---

# 🧠 1. TYPES OF MACHINE LEARNING

### 🔹 Supervised Learning

* Data is labeled
* Example: House price prediction

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()
model.fit(X_train, y_train)
pred = model.predict(X_test)
```

---

### 🔹 Unsupervised Learning

* No labels
* Example: Customer segmentation

```python
from sklearn.cluster import KMeans

model = KMeans(n_clusters=3)
model.fit(X)
```

---

### 🎯 Interview Q

**Q. Difference between supervised & unsupervised?**
👉 Supervised → labeled data
👉 Unsupervised → unlabeled data

---

# 📊 2. DATA HANDLING

### 📂 Load CSV

```python
import pandas as pd
df = pd.read_csv('data.csv')
```

### 🌐 API Data

```python
import requests

res = requests.get(url)
data = res.json()
df = pd.DataFrame(data)
```

---

### 🎯 Interview Q

**Q. Why data preprocessing is important?**
👉 Raw data is messy → model needs clean data

---

# 🧹 3. DATA CLEANING

```python
df.dropna(inplace=True)
df.fillna(df.mean(), inplace=True)
df.duplicated().sum()
```

---

### 🎯 Interview Q

**Q. How to handle missing values?**
👉 Drop or fill (mean/median/mode)

---

# 📈 4. EDA (Exploratory Data Analysis)

```python
df.describe()
df.corr()
```

---

### 🎯 Interview Q

**Q. Why EDA important?**
👉 Understand patterns before modeling

---

# ⚙️ 5. FEATURE ENGINEERING

### 🔹 Encoding

```python
pd.get_dummies(df['gender'])
```

### 🔹 Scaling

```python
from sklearn.preprocessing import StandardScaler

scaler = StandardScaler()
X_scaled = scaler.fit_transform(X)
```

---

### 🎯 Interview Q

**Q. Why scaling needed?**
👉 Algorithms sensitive to feature range

---

# 🤖 6. MACHINE LEARNING MODELS

---

## 📌 Linear Regression

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()
model.fit(X_train, y_train)
```

---

### 🎯 Interview Q

**Q. When use Linear Regression?**
👉 Continuous output

---

## 📌 Logistic Regression

```python
from sklearn.linear_model import LogisticRegression

model = LogisticRegression()
model.fit(X_train, y_train)
```

---

### 🎯 Interview Q

**Q. Why called regression but used for classification?**
👉 Uses sigmoid function

---

## 📌 Decision Tree

```python
from sklearn.tree import DecisionTreeClassifier

model = DecisionTreeClassifier()
model.fit(X_train, y_train)
```

---

### 🎯 Interview Q

**Q. Advantage of Decision Tree?**
👉 Easy to interpret

---

## 📌 Random Forest

```python
from sklearn.ensemble import RandomForestClassifier

model = RandomForestClassifier()
model.fit(X_train, y_train)
```

---

### 🎯 Interview Q

**Q. Why better than Decision Tree?**
👉 Reduces overfitting

---

## 📌 KNN

```python
from sklearn.neighbors import KNeighborsClassifier

model = KNeighborsClassifier(n_neighbors=5)
model.fit(X_train, y_train)
```

---

### 🎯 Interview Q

**Q. Disadvantage of KNN?**
👉 Slow for large data

---

# 📉 7. MODEL EVALUATION

```python
from sklearn.metrics import accuracy_score

accuracy_score(y_test, pred)
```

---

### 🎯 Interview Q

**Q. Accuracy vs Precision?**
👉 Accuracy → overall correct
👉 Precision → correct positives

---

# 🚀 8. ADVANCED CONCEPTS

---

### 🔹 Overfitting & Underfitting

* Overfitting → memorizes data
* Underfitting → poor learning

---

### 🔹 Cross Validation

```python
from sklearn.model_selection import cross_val_score

cross_val_score(model, X, y, cv=5)
```

---

### 🎯 Interview Q

**Q. Why cross validation?**
👉 Better model evaluation

---

### 🔹 Pipeline

```python
from sklearn.pipeline import Pipeline

pipe = Pipeline([
    ('scaler', StandardScaler()),
    ('model', LogisticRegression())
])
```

---

### 🎯 Interview Q

**Q. What is Pipeline?**
👉 Automates steps

---

# 🧩 REAL-WORLD QUESTIONS

---

**Q. Data is huge?**
👉 Use sampling / chunks

---

**Q. Data imbalance?**
👉 Use resampling

---

**Q. Feature selection?**
👉 Remove irrelevant features

---

# 🔥 MOST IMPORTANT INTERVIEW QUESTIONS

---

### 🔹 Q1. What is Bias vs Variance?

👉 Bias → error due to assumptions
👉 Variance → error due to sensitivity

---

### 🔹 Q2. What is Regularization?

👉 Prevents overfitting

---

### 🔹 Q3. What is Confusion Matrix?

👉 Shows TP, FP, TN, FN

---

### 🔹 Q4. What is F1 Score?

👉 Balance of precision & recall

---

# 📂 PROJECTS

* Movie Recommendation System 🎬
* ML Classification Projects
* API Data Projects

---

# ⭐ FINAL TAKEAWAY

✔ Data cleaning is 70% of ML
✔ Feature engineering is key
✔ Model evaluation matters
✔ Practice daily

---

## 🙌 Author

Tanisha 🚀
Future ML Engineer 💡

