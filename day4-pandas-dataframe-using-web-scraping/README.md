# 🌐 Data Collection & Processing Interview Guide

> 🧠 Focus: API → JSON → Web Scraping → Pandas DataFrame

---

# 📌 Topics Covered

* API Handling
* JSON Data
* Pandas DataFrame
* Web Scraping (BeautifulSoup)
* Data Cleaning

---

# 🧠 🔰 BASIC QUESTIONS

---

### 🔹 Q1. What is an API?

👉 API (Application Programming Interface) allows different systems to communicate and exchange data.

---

### 🔹 Q2. What is `requests` library?

👉 It is used to send HTTP requests (GET, POST) and fetch data from APIs.

---

### 🔹 Q3. What is JSON?

👉 JSON is a lightweight data format used to store and transfer data in key-value pairs.

---

### 🔹 Q4. Why convert API data to DataFrame?

👉 Because DataFrame provides structured format which is easy to analyze and process.

---

### 🔹 Q5. What is Web Scraping?

👉 Extracting data from websites using HTML parsing.

---

### 🔹 Q6. What is BeautifulSoup?

👉 A Python library used to parse HTML and extract data from web pages.

---

### 🔹 Q7. What is a DataFrame?

👉 A tabular data structure with rows and columns (like Excel table).

---

---

# ⚙️ 🟡 INTERMEDIATE QUESTIONS

---

### 🔹 Q8. What is `requests.get()`?

👉 Sends a GET request to a server and retrieves data.

---

### 🔹 Q9. What is a status code?

👉 It indicates the result of an HTTP request (200 = success, 404 = not found).

---

### 🔹 Q10. What does `.json()` do?

👉 Converts API response into Python dictionary.

---

### 🔹 Q11. What is `pd.DataFrame()`?

👉 Converts structured data (list/dict) into tabular format.

---

### 🔹 Q12. What is `json_normalize()`?

👉 Converts nested JSON into flat table structure.

---

### 🔹 Q13. What is `.text` in requests?

👉 Returns raw HTML content as string.

---

### 🔹 Q14. What is `.find()` in BeautifulSoup?

👉 Extracts first matching HTML element.

---

### 🔹 Q15. What is `.find_all()`?

👉 Extracts all matching elements.

---

### 🔹 Q16. Why use `.strip()`?

👉 Removes unwanted spaces and newline characters.

---

### 🔹 Q17. Why loops used in scraping?

👉 To extract repeated elements like company lists.

---

---

# 🚀 🔴 ADVANCED QUESTIONS

---

### 🔹 Q18. How do you handle nested JSON data?

👉 Use `json_normalize()` or manually flatten the structure.

---

### 🔹 Q19. How to scrape multiple pages?

👉 Use loop + dynamic URL (pagination).

---

### 🔹 Q20. What is pagination in APIs/websites?

👉 Data is divided into multiple pages and fetched sequentially.

---

### 🔹 Q21. Why use try-except in scraping?

👉 To handle missing tags or errors without crashing the program.

---

### 🔹 Q22. What is np.nan?

👉 Represents missing values in dataset.

---

### 🔹 Q23. What are HTTP methods?

👉 GET, POST, PUT, DELETE.

---

### 🔹 Q24. What is API latency?

👉 Time delay between request and response.

---

### 🔹 Q25. Why `append()` is not recommended in loop?

👉 It is slow; better to use list + concat.

---

### 🔹 Q26. Difference between `.text` and `.content`?

👉 `.text` → string
👉 `.content` → raw bytes

---

### 🔹 Q27. What is HTML parsing?

👉 Converting raw HTML into structured tree format.

---

---

# 🧩 REAL-WORLD QUESTIONS

---

### 🔹 Q28. API returns huge data?

👉 Use pagination or filters to reduce load.

---

### 🔹 Q29. API fails or returns error?

👉 Check status code and retry request.

---

### 🔹 Q30. Website structure changes?

👉 Update scraping logic (selectors).

---

### 🔹 Q31. Missing data in scraping?

👉 Use try-except and fill with `np.nan`.

---

### 🔹 Q32. Scraping gets blocked?

👉 Use headers, delay requests, or proxies.

---

### 🔹 Q33. Data not structured properly?

👉 Clean and transform using pandas.

---

### 🔹 Q34. Duplicate data?

👉 Use `drop_duplicates()`.

---

---

# 🔥 TRICKY QUESTIONS

---

### 🔹 Q35. API vs Web Scraping?

👉 API → structured & reliable
👉 Scraping → unstructured & fragile

---

### 🔹 Q36. Why JSON preferred over XML?

👉 Lightweight, faster, easier to parse.

---

### 🔹 Q37. Why DataFrame over list?

👉 Better analysis, filtering, and operations.

---

### 🔹 Q38. What if HTML tag not found?

👉 Handle using try-except or condition checks.

---

### 🔹 Q39. Why scraping sometimes fails?

👉 Dynamic content (JavaScript) or anti-bot protection.

---

### 🔹 Q40. Difference: structured vs semi-structured data?

👉 Structured → tables
👉 Semi-structured → JSON

---

---

# ⭐ FINAL TAKEAWAYS

✔ APIs are more reliable than scraping
✔ Always inspect HTML before scraping
✔ Use try-except for robust code
✔ Convert data into DataFrame for analysis
✔ Optimize code for performance

---

## 🙌 Author

Tanisha 🚀
Aspiring Data Analyst
