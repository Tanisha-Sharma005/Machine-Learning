# 📊 Working with CSV Files using Pandas

> 🧠 Complete Interview Guide (Basic → Advanced) for Machine Learning 

---

## 📌 📚 Topics Covered

- CSV & TSV files
- read_csv()
- usecols, dtype
- encoding issues
- index_col
- parse_dates
- handling large datasets
- real-world data problems

---

# 🧠 🔰 BASIC INTERVIEW QUESTIONS

### 🔹 Q1. What is a CSV file?
**Answer:**  
CSV (Comma Separated Values) is a text file used to store tabular data where values are separated by commas.

---

### 🔹 Q2. What is pandas?
**Answer:**  
Pandas is a Python library used for data manipulation and analysis, especially for structured data.

---

### 🔹 Q3. What is a DataFrame?
**Answer:**  
A DataFrame is a 2D table-like data structure with rows and columns, similar to an Excel sheet.

---

### 🔹 Q4. What does `read_csv()` do?
**Answer:**  
It reads a CSV file and converts it into a pandas DataFrame.

---

### 🔹 Q5. What is the default delimiter in CSV?
**Answer:**  
Comma `,`

---

### 🔹 Q6. Difference between CSV and TSV?
**Answer:**  
- CSV → comma separated  
- TSV → tab separated  

---

### 🔹 Q7. What is a Series?
**Answer:**  
A Series is a 1D data structure representing a single column.

---

---

# ⚙️ 🟡 INTERMEDIATE QUESTIONS

### 🔹 Q8. What is `usecols`?
**Answer:**  
It is used to load only selected columns, improving performance and saving memory.

---

### 🔹 Q9. What is `dtype`?
**Answer:**  
It defines the data type of columns and helps in memory optimization.

---

### 🔹 Q10. What is `index_col`?
**Answer:**  
It sets a column as the index of the DataFrame for faster access.

---

### 🔹 Q11. What is encoding?
**Answer:**  
Encoding defines how characters are stored in a file (e.g., UTF-8, latin-1).

---

### 🔹 Q12. What is `parse_dates`?
**Answer:**  
It converts columns into datetime format.

---

### 🔹 Q13. What is `nrows`?
**Answer:**  
It limits the number of rows to be read.

---

### 🔹 Q14. What is `skiprows`?
**Answer:**  
It skips specified rows while reading the file.

---

### 🔹 Q15. What is `on_bad_lines='skip'`?
**Answer:**  
It skips rows with incorrect formatting.

---

---

# 🚀 🔴 ADVANCED QUESTIONS

### 🔹 Q16. What happens internally in `read_csv()`?
**Answer:**  
- File is opened  
- Data is parsed using delimiter  
- Converted into DataFrame  
- Data types are inferred automatically  

---

### 🔹 Q17. How to handle large CSV files?
**Answer:**  
- Use `usecols`  
- Use `dtype` optimization  
- Use `chunksize`  
- Use `nrows`  

---

### 🔹 Q18. What is memory optimization?
**Answer:**  
Reducing RAM usage by:
- Selecting required columns  
- Using correct data types  

---

### 🔹 Q19. What is chunk processing?
**Answer:**  
Reading large files in smaller parts using `chunksize`.

---

### 🔹 Q20. Difference between `loc` and `iloc`?
**Answer:**  
- loc → label-based indexing  
- iloc → position-based indexing  

---

---

# 🧩 🟣 REAL-WORLD SCENARIO QUESTIONS

### 🔹 Q21. File is too large to fit in RAM. What will you do?
**Answer:**  
- Use chunk processing  
- Use Dask or PySpark  
- Load only required columns  

---

### 🔹 Q22. CSV file has encoding error. How to fix?
**Answer:**  
```python
pd.read_csv(file, encoding='latin-1')
