# 🐍 Python for Data Analytics — Professional Learning Journey

## About This Repository

This repository documents my structured journey through the **Python for Data Analytics Bootcamp** .

The focus of this program is not only learning Python syntax, but developing the ability to:

> **Design, automate, and scale data workflows in real-world analytics environments**

---

## Objectives

Through this course, I am building the ability to:

* Automate repetitive analytical tasks
* Work with structured and large-scale datasets
* Build reproducible data workflows
* Combine SQL and Python effectively
* Develop production-ready analytical thinking

---

## Core Concept

> Python is not a replacement for SQL or Excel.
> It is a tool for **controlling the entire data workflow**.

---

## Tech Stack

* Python 3.x
* Miniconda (environment management)
* Jupyter Notebook / VS Code
* pandas, numpy
* matplotlib, seaborn
* scikit-learn

---

## Course Structure

The course is structured into **12 progressive sessions**:

## 📚 Sessions

| Session | Topic | Content |
|--------|------|---------|
| 01 | Foundations | [Read](#-session-01--foundations) |
| 02 | Python Fundamentals | [Read](#-session-02--python-fundamentals-for-data-analytics) |
| 03 | Pandas & Data Workflow | [Read](#-session-03--introduction-to-pandas--data-workflow) |
---

# 🧩 Session 01 — Foundations

## 🔹 Overview

Session 01 introduces the **fundamental shift from manual data analysis to automated workflows**.

---

## 🔹 Key Concepts

### 1. SQL vs Python

| SQL           | Python           |
| ------------- | ---------------- |
| Declarative   | Imperative       |
| What you want | How to do it     |
| Data querying | Workflow control |

👉 SQL retrieves data
👉 Python defines what happens next

---

### 2. Analytical Mindset Shift

Transition:

* From manual tools → automation
* From queries → workflows
* From analyst → system thinker

---

### 3. Data Types

Core types:

```python
int      # 10
float    # 3.14
str      # "Alice"
bool     # True / False
```

⚠️ Incorrect data types lead to incorrect analysis.

---

### 4. Variables

Variables are **named references to values in memory**:

```python
price = 100
quantity = 3
revenue = price * quantity
```

Used to:

* Store data
* Reuse values
* Build logic

---

### 5. Automation

Example:

```python
df = df[df["price"] > 0]
```

Instead of repeating manual steps →
👉 Define logic once → execute automatically

---

### 6. Reproducibility

Python ensures:

* Transparent workflows
* Repeatable results
* Collaboration readiness

---

### 7. Notebook Workflow

Best practices:

* One step per cell
* Markdown for explanations
* Code for execution

👉 Notebook = analysis story

---

### 8. Python Ecosystem

Key libraries:

* pandas → data manipulation
* numpy → numerical operations
* matplotlib / seaborn → visualization

---

### 9. Environment Management

Using Miniconda:

```bash
conda create -n myenv python=3.13
conda activate myenv
pip install pandas
```

👉 One project = one environment

---

### 10. Reproducibility via requirements.txt

```txt
pandas==2.2.2
numpy==1.26.4
```

```bash
pip install -r requirements.txt
```

Ensures:

* Consistent environments
* Easy collaboration

---

## 🔥 Key Takeaways

* Python enables automation, scalability, and control
* SQL and Python are complementary
* Data types directly affect correctness
* Variables are the foundation of logic
* Environments are critical for professional workflows

---

## 📁 Project Structure

```bash
data_analytics_with_python/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
├── imgs/
├── docs/
├── gitignore
├── requirements.txt
├── README.md
```

---

## 📈 Progress

* [x] Session 01 — Foundations
* [ ] Session 02 — Data Structures
* [ ] Session 03 — Control Flow
* [ ] Session 04 — Functions
* [ ] Session 05 — File Handling
* [ ] Session 06 — NumPy
* [ ] Session 07 — Pandas
* [ ] Session 08 — Data Cleaning
* [ ] Session 09 — Visualization
* [ ] Session 10 — Workflows
* [ ] Session 11 — Automation
* [ ] Session 12 — Final Project

---

## Next Step

➡️ Session 02: Data Structures
Focus: Lists, Dictionaries, Data Organization

---

## 💡 Final Note

This repository reflects a transformation:

> From running queries → to building data systems

# 🧩 Session 02 — Python Fundamentals for Data Analytics

## 🔹 Overview

Session 02 builds the **core programming foundation required for analytical thinking in Python**.

The focus is not just syntax, but understanding how to:

> **Represent, transform, and analyze data using programmatic logic**

This session marks the transition from:

* Writing simple code → to **thinking in data transformations**

---

##  What I Can Do After This Session

After completing this session, I can:

- Perform core analytical computations using Python
- Structure raw data into lists, dictionaries, and tabular formats
- Apply conditional logic for filtering and segmentation
- Iterate over datasets and compute aggregations
- Write concise transformations using list comprehension
- Transition from raw Python structures to pandas DataFrames
- Perform basic data manipulation and filtering

---

## 🔹 Key Concepts

### 1. Arithmetic & Boolean Logic

Python supports fundamental operations used in all analytical workflows:

```python
r = 100
t = 0.2
total = r * (1 + t)
```

Boolean logic enables decision-making:

```python
100 > 50
100 == 50
100 != 50
```

Logical operators:

* `and`
* `or`
* `not`

👉 These form the basis of **filtering and rule-based analysis**

---

### 2. Core Data Structures

#### List — Ordered Data

```python
sales = [100, 200, 150]
```

Used for:

* Time series
* Measurements
* Sequential data

---

#### Tuple — Immutable Data

```python
coordinates = (40.18, 44.51)
```

Used for:

* Fixed values
* Constants
* Safe data storage

---

#### Set — Unique Values

```python
customer_ids = {1, 2, 3, 3}
```

Key features:

* Removes duplicates
* Fast membership checks
* Supports set operations

Used for:

* Deduplication
* Data validation
* Segment comparison

---

#### Dictionary — Structured Records

```python
customer = {
    "name": "Anna",
    "revenue": 150,
    "city": "Yerevan"
}
```

Used for:

* Representing entities (rows)
* Key-value relationships
* Building structured datasets

---

### 3. From Structures to Tables

A list of dictionaries represents tabular data:

```python
customers = [
    {"name": "Anna", "revenue": 150},
    {"name": "David", "revenue": 220}
]
```

👉 This is the conceptual bridge to **DataFrames**

---

### 4. Introduction to pandas DataFrame

A DataFrame is conceptually:

* A collection of columns
* Each column behaves like a labeled list

```python
import pandas as pd

df = pd.DataFrame({
    "name": ["Anna", "David"],
    "revenue": [150, 220]
})
```

Basic operations:

* Column selection
* Row filtering
* Feature creation
* Column removal

👉 Mirrors SQL operations (`SELECT`, `WHERE`)

---

### 5. Conditional Statements (Decision Logic)

```python
if revenue > 100:
    print("High revenue")
else:
    print("Normal revenue")
```

Key principles:

* Conditions evaluate to `True` or `False`
* Indentation defines execution blocks
* `elif` enables multi-branch logic

Used for:

* Filtering
* Segmentation
* Rule-based scoring

---

### 6. Loops (Iteration)

```python
for value in sales:
    print(value)
```

Used for:

* Iterating over datasets
* Applying rules
* Aggregation

Example:

```python
total = 0
for value in sales:
    total += value
```

---

### 7. Combining Logic and Iteration

```python
for value in sales:
    if value > 120:
        print(value)
```

👉 Represents row-by-row filtering logic

---

### 8. range() and Control Flow

```python
for i in range(5):
    print(i)
```

Used for:

* Controlled iteration
* Index-based logic

---

### 9. Nested Loops

```python
for i in range(3):
    for j in range(2):
        print(i, j)
```

Used for:

* Multi-dimensional data
* Pairwise operations

⚠️ Increased complexity → impacts performance

---

### 10. List Comprehension (Efficient Transformation)

```python
new_sales = [value * 1.2 for value in sales]
```

With condition:

```python
high_sales = [value for value in sales if value > 120]
```

With transformation:

```python
labels = ["High" if v > 120 else "Low" for v in sales]
```

👉 Combines:

* Iteration
* Filtering
* Transformation

---

### 11. Mutable vs Immutable Objects

**Mutable:**

* list, dict, set, DataFrame

**Immutable:**

* int, float, str, tuple

Why it matters:

* Prevents unintended changes
* Avoids hidden bugs
* Ensures predictable behavior

---

## 🔄 Analytical Perspective

This session establishes the core mapping between Python and analytics:

| Python Concept     | Analytics Equivalent |
| ------------------ | -------------------- |
| if                 | WHERE clause         |
| loop               | row iteration        |
| sum logic          | aggregation          |
| list comprehension | transformation       |
| dictionary         | record               |
| DataFrame          | table                |

---

## 🔥 Key Takeaways

* Data structures define how information is organized
* Conditional logic enables decision-making
* Loops enable scalable computation
* List comprehension enables clean transformations
* DataFrames formalize structured analysis

---

## 📈 Progress

* [x] Session 01 — Foundations
* [x] Session 02 — Python Fundamentals
* [ ] Session 03 — Control Flow (Advanced)
* [ ] Session 04 — Functions
* [ ] Session 05 — File Handling
* [ ] Session 06 — NumPy
* [ ] Session 07 — Pandas
* [ ] Session 08 — Data Cleaning
* [ ] Session 09 — Visualization
* [ ] Session 10 — Workflows
* [ ] Session 11 — Automation
* [ ] Session 12 — Final Project

---

## Next Step

➡️ Session 03: Pandas + Data Workflow (Advanced)
Focus: Functions, deeper logic, and reusable workflows

---

## 💡 Final Note

This session completes the transition:

> From writing Python code → to thinking in data logic and transformations


# 🧩 Session 03 — Introduction to Pandas & Data Workflow

## 🔹 Overview
Session 03 introduces **pandas** as the core tool for data analysis and builds the first end-to-end data workflow.

**The focus shifts from:**
> Writing Python logic → to working with real datasets

**This session establishes the foundation for:**
* Exploring, cleaning, transforming, and exporting structured data.

---

## 🎯 What I Can Do After This Session
After completing this session, I can:
* **Load** large-scale datasets into pandas DataFrames.
* **Perform** structured data exploration (EDA).
* **Clean and transform** raw data into usable formats.
* **Create** analytical features from existing columns.
* **Handle** missing values correctly.
* **Reshape** datasets when necessary.
* **Export** processed datasets for further analysis.

---

## 🔹 Key Concepts

### 1. Pandas Core Data Structures
* **Series**: 1-dimensional labeled array (Values + Index).
* **DataFrame**: 2-dimensional table (Rows + Columns + Values). Equivalent to a SQL table or Excel sheet.

### 2. Data Import
```python
import pandas as pd

df_orders = pd.read_csv("../data/raw/orders.csv")
df_products = pd.read_csv("../data/raw/products.csv")

   Key principle: Always validate data immediately after loading.


## 3. Data Exploration (EDA)

Core inspection methods:

| Method | Description |
|---|---|
| `df.head()` / `df.tail()` | View first / last rows |
| `df.columns` | Column names |
| `df.info()` | General info (types, nulls) |
| `df.dtypes` | Data type of each column |
| `df.describe()` | Statistical summary |

---

## 4. Data Wrangling (Cleaning & Structuring)

- **Dropping columns:**
  ```python
  df.drop(columns=["eval_set"])
  ```

- **Renaming columns:**
  ```python
  df.rename(columns={"eval_set": "dataset_type"})
  ```

- **Changing types:**
  ```python
  df["order_id"] = df["order_id"].astype("int64")
  ```

---

## 5. Feature Engineering

Creating business-ready insights:

```python
# Boolean flags
df["is_weekend"] = df["order_dow"].isin([0, 6])

# Categorization using apply
df["order_frequency_category"] = df["order_number"].apply(
    lambda x: "New" if x == 1 else "Low" if x <= 5 else "High"
)
```

---

## 6. Handling Missing Values

```python
df["days_since_prior_order"] = df["days_since_prior_order"].fillna(0)
```

> **Key principle:** Missing data must be explicitly handled before analysis.

---

## 7. Vectorization vs `apply()`

| Approach | Efficiency |
|---|---|
| ✅ Preferred (Vectorized): `df["order_hour_of_day"] < 12` | Fast and scalable |
| ⚠️ Less efficient: `df["col"].apply(lambda x: ...)` | Avoid when possible |

> **Key principle:** Vectorized operations are faster and more scalable.

---

## 8. Data Reshaping

- **Transpose** (Convert wide → long format or fix structure):
  ```python
  df.T
  ```

---

## 9. Exporting Data

```python
df.to_csv("../data/processed/orders_cleaned.csv", index=False)
```

> **Key principle:** Processed data should be saved separately from raw data.

---

## 🔄 Analytical Perspective

| Action | Purpose |
|---|---|
| `head` / `tail` | Quick inspection |
| `info` / `dtypes` | Structure & data types |
| `describe` | Statistical overview |
| `drop` / `rename` | Cleaning |
| `astype` | Data correctness |
| Feature creation | Business logic |
| `fillna` | Data reliability |
| `to_csv` | Workflow output |

---

## 🔥 Key Takeaways

- Pandas is the core tool for data analysis in Python.
- Every analysis starts with Structured Exploration (EDA).
- Data must be cleaned before it can be analyzed.
- Feature engineering creates business value.
- Vectorized operations are essential for performance.

---

## 📈 Progress (Updated)

- [x] Session 01 — Foundations
- [x] Session 02 — Python Fundamentals
- [x] Session 03 — Pandas & Data Workflow
- [ ] Session 04 — Functions
- [ ] Session 05 — File Handling
- [ ] Session 06 — NumPy
- [ ] Session 07 — Advanced Pandas
- [ ] Session 08 — Data Cleaning (Advanced)
- [ ] Session 09 — Visualization
- [ ] Session 10 — Workflows
- [ ] Session 11 — Automation
- [ ] Session 12 — Final Project

**Next Step:** ➡️ Session 04: Functions (Reusable logic & modular code)

---

> 💡 **Final Note:** This session marks a major transition from writing basic Python code to building real data pipelines.


