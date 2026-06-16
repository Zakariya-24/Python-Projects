# Python-Projects
# Python Data Technician Portfolio

This repository contains my **Week 6 Python work** from the Data Technician programme. The project includes Python exercises, Google Colab notebooks, Jupyter notebooks, and beginner data analysis tasks using **Pandas**.

---

## 📌 Project Overview

The aim of this project was to practise Python programming and understand how Python can be used for data analysis.

The work covered Python basics such as variables, loops, if statements, functions, lists, user input, and problem-solving. It also introduced **Pandas**, which is one of the main Python libraries used for working with structured data.

---

## 🔗 Google Colab Notebooks

I used **Google Colab** to complete the Python tasks because it allows code to be written, tested and explained in one place. Colab is useful for learning Python because it runs in the browser, does not need software installed, and makes it easy to share notebooks with trainers or other users.

Each Colab notebook contains Python code cells and written notes. This made it easier to practise the code, run each section step by step, check the output, and explain what the code was doing.

---

### 📘 Day 1: Python Exercises

**Colab link:**
https://colab.research.google.com/drive/1X2y7wcJ768lPnnq4HEOK2hpeefz3Bzl5?usp=sharing

This notebook focused on beginner Python skills. I used it to practise writing basic Python code, using variables, printing outputs, and understanding how code runs in separate cells.

---

### 📘 Day 2: Python Exercises

**Colab link:**
https://colab.research.google.com/drive/1FMs6Dqg_tTSqn0wAuTa0aTX_vkYwkEJM?usp=sharing

This notebook helped me build on the basics by using conditions, loops and simple problem-solving. It supported tasks such as the FizzBuzz challenge, where I used `for` loops and `if` statements to control the output.

---

### 📘 Day 4: Pandas DataFrames

**Colab link:**
https://colab.research.google.com/drive/1ZLG3LgzHUgYfVlLzs8W2OpBugHWRBTKP?usp=sharing

This notebook introduced **Pandas**, which is used for working with data in tables. I used Colab to create and view DataFrames, check rows and columns, and understand how data can be organised using Python.

---

### 📘 Day 4: Pandas Dataset Task

**Colab link:**
https://colab.research.google.com/drive/1OIlNFt7vYRuikgRUw8HemN543jdeM8lM?usp=sharing

This notebook focused on using a real dataset. I practised importing data, checking the structure of the dataset, viewing the first few rows, and exploring the information using Pandas commands such as `head()`, `info()` and `describe()`.

---

### 📘 Day 4: Additional Dataset Task

**Colab link:**
https://colab.research.google.com/drive/1SzWwpS86Eju3tp_EDpBKFmYqFseWVam_?usp=sharing

This notebook gave me more practice with dataset analysis. I used it to improve my confidence with filtering, sorting, checking missing values and preparing data for further analysis.

---

## 💡 Why Google Colab Was Useful

Google Colab helped me because I could write code, run it instantly and see the output underneath each cell. This made it easier to test small sections of code and fix mistakes.

It was also useful for learning Pandas because tables can be displayed clearly inside the notebook. This made it easier to understand the dataset before cleaning or analysing it.

Overall, using Google Colab helped me practise Python in a more organised way and made it easier to show my work clearly.

---

## 📁 Files Included

* `Zakariya_Notebook.ipynb`
* `Zakariya_Notebook_Part_2.ipynb`
* `Zakariya_Notebook_Part_3.ipynb`
* `Data_Technician_Workbook_Week_6 - 2026.docx`

---

## 🧠 Python Skills Practised

* Python syntax
* Variables and data types
* Loops
* If statements
* Functions
* Lists and dictionaries
* User input
* Problem-solving
* FizzBuzz challenge

---

## ✅ FizzBuzz Task

One of the tasks was to create the classic **FizzBuzz** challenge using Python.

The program goes through numbers from 1 to 100:

* If the number is divisible by 3, it prints `fizz`
* If the number is divisible by 5, it prints `buzz`
* If the number is divisible by both 3 and 5, it prints `fizzbuzz`
* Otherwise, it prints the number

```python
for number in range(1, 101):
    if number % 3 == 0 and number % 5 == 0:
        print("fizzbuzz")
    elif number % 3 == 0:
        print("fizz")
    elif number % 5 == 0:
        print("buzz")
    else:
        print(number)
```

---

## 🐼 Using Pandas

A key part of this project was learning how to use **Pandas** for data analysis. Pandas is useful because it allows data to be stored, cleaned, filtered and analysed in a table format, similar to working with spreadsheets.

I used Pandas in Google Colab and Jupyter notebooks to work with datasets. This helped me understand how Python can be used to explore data instead of only writing basic programs.

Some of the Pandas skills practised include:

* Importing the Pandas library
* Creating DataFrames
* Reading CSV files
* Viewing the first and last rows of a dataset
* Checking the shape of a dataset
* Viewing column names
* Selecting specific columns
* Filtering rows based on conditions
* Sorting data
* Checking for missing values
* Removing or handling missing data
* Creating simple summaries
* Understanding data types

Example Pandas code:

```python
import pandas as pd

df = pd.read_csv("data.csv")

print(df.head())
print(df.info())
print(df.describe())
```

---

## 🧪 Advanced Python Example

I also included a more advanced Python example using **Pandas**. The code loads a CSV file, cleans the data, removes duplicates, handles missing values, groups sales by region and category, filters high sales records, and exports a summary file.

This shows how Python can be used for real data technician tasks such as data cleaning, analysis and reporting.

```python
import pandas as pd

df = pd.read_csv("sales_data.csv")

df = df.drop_duplicates()
df = df.fillna("Unknown")

sales_summary = df.groupby(["Region", "Category"])["Sales"].sum().reset_index()
sales_summary = sales_summary.sort_values(by="Sales", ascending=False)

high_sales = df[df["Sales"] >= 500]

print(sales_summary)
print(high_sales)

sales_summary.to_csv("sales_summary.csv", index=False)
```

---

## 📊 Why Pandas Is Useful

Pandas is useful for data analysis because it makes it easier to work with large datasets. Instead of checking data manually, Pandas allows users to quickly clean, filter and summarise information.

For example, Pandas can be used to answer questions such as:

* How many rows and columns are in the dataset?
* Are there any missing values?
* Which values are the highest or lowest?
* What is the average value in a column?
* Which rows match a certain condition?
* How can the data be cleaned before visualisation?

This makes Pandas an important tool for data technicians because clean and organised data is needed before creating dashboards, reports or insights.

---

## 🔍 What I Learned

This project helped me build confidence with Python basics and understand how programming logic works.

I learned how to use loops and conditions to solve problems, and how Pandas can be used to explore and clean data. I also practised working in Google Colab and Jupyter notebooks, which is useful for writing code, testing outputs and explaining each step clearly.

Using Pandas helped me see how Python can be applied to real data tasks. It showed me how to move from basic coding into data analysis, where the goal is to find patterns, clean data and prepare information for reporting.

---

## 🛠️ Tools Used

* Python
* Google Colab
* Jupyter Notebook
* Pandas
* CSV files

---

