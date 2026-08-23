# 🐼 Pandas & Data Analysis with Python

A practical repository for learning **Pandas and Data Analysis with Python** through Jupyter Notebooks, datasets, and mini projects.

This repository covers the fundamental concepts of the **Pandas library**, including Series, DataFrames, data cleaning, merging, grouping, aggregation, pivot tables, data transformation, and feature extraction.

It is designed for beginners and students who want to build a strong foundation in **Data Science, Data Analytics, and Machine Learning**.

---

## 📌 About Pandas

**Pandas** is an open-source Python library used for **data manipulation and data analysis**.

It provides powerful data structures such as:

* **Series** – One-dimensional labeled data
* **DataFrame** – Two-dimensional tabular data

Pandas makes it easy to:

* Load datasets
* Clean data
* Handle missing values
* Filter data
* Sort data
* Combine datasets
* Group and summarize data
* Transform data
* Perform statistical operations
* Prepare data for Machine Learning

---

# 📚 Topics Covered

## 1. Series

**Notebook:** `1. Series.ipynb`

This notebook introduces the Pandas Series data structure.

### Topics:

* Creating Series
* Series using Lists
* Series using NumPy Arrays
* Series using Dictionaries
* Indexing
* Slicing
* Basic Series operations

A Series is a **one-dimensional labeled data structure**.

Example:

```python
import pandas as pd

data = pd.Series([10, 20, 30, 40, 50])

print(data)
```

---

## 2. DataFrame

**Notebook:** `2. Data Frame.ipynb`

A DataFrame is a **two-dimensional table-like data structure** consisting of rows and columns.

### Topics:

* Creating DataFrames
* Selecting columns
* Selecting rows
* Adding columns
* Removing columns
* Indexing
* DataFrame operations

Example:

```python
import pandas as pd

data = {
    "Name": ["Monu", "Rahul", "Amit"],
    "Age": [21, 22, 20]
}

df = pd.DataFrame(data)

print(df)
```

---

## 3. Missing Data

**Notebook:** `3. MissingData.ipynb`

Real-world datasets often contain missing or incomplete values.

This notebook demonstrates how to identify and handle missing data.

### Topics:

* Detecting missing values
* `isnull()`
* `notnull()`
* `dropna()`
* `fillna()`
* Replacing missing values

Example:

```python
df.isnull()

df.dropna()

df.fillna(0)
```

Proper handling of missing values is an important step in **Data Cleaning and Machine Learning preprocessing**.

---

## 4. Merging, Joining & Concatenation

**Notebook:** `4. MergingjoiningandConcatination.ipynb`

This notebook explains how multiple DataFrames can be combined.

### Important functions:

* `merge()`
* `join()`
* `concat()`

### Types of Joins:

* Inner Join
* Left Join
* Right Join
* Outer Join

Example:

```python
result = pd.merge(df1, df2, on="ID")
```

These operations are useful when working with data stored across multiple tables or datasets.

---

## 5. GroupBy & Aggregation

**Notebook:** `5. GroupBy_and_Aggregation.ipynb`

The `groupby()` function is used to divide data into groups and perform calculations on those groups.

### Common aggregation functions:

* `sum()`
* `mean()`
* `count()`
* `min()`
* `max()`

Example:

```python
df.groupby("Category")["Sales"].mean()
```

This is commonly used for **data summarization and business analytics**.

---

## 6. Pivot Table

**Notebook:** `6. Pivot_Table.ipynb`

Pivot tables provide a convenient way to summarize and analyze large datasets.

### Topics:

* Creating pivot tables
* Rows
* Columns
* Values
* Aggregation functions

Example:

```python
pd.pivot_table(
    df,
    values="Sales",
    index="Category",
    aggfunc="mean"
)
```

Pivot tables are especially useful for **reporting and exploratory data analysis**.

---

## 7. Pandas Operations

**Notebook:** `7. Operations.ipynb`

This notebook covers different operations used to transform and analyze Pandas data.

### Topics:

* Mathematical operations
* Statistical operations
* `apply()`
* `map()`
* `applymap()`
* Sorting
* Ranking
* Data transformation

These operations help convert raw data into useful information.

---

# 📊 Mini Projects

## 8. Feature Extraction Project

**Notebook:** `FeatureExtraction_Project-01.ipynb`

This project demonstrates basic **feature extraction** techniques.

Feature extraction converts raw information into meaningful features that can be used for analysis or Machine Learning.

### Importance:

```text
Raw Data
   ↓
Feature Extraction
   ↓
Useful Features
   ↓
Machine Learning Model
```

Feature extraction is an important part of the **Machine Learning preprocessing pipeline**.

---

## 9. Countries Data Analysis

**Notebook:** `Countries_Project-02.ipynb`

This project performs data analysis using country-related information.

### Concepts demonstrated:

* Loading data
* Filtering
* Grouping
* Aggregation
* Data manipulation
* Extracting insights

### Dataset:

```text
Countries.csv
```

This project provides practical experience working with a real-world-style dataset.

---

# 📁 Datasets

The repository includes datasets used for practical analysis.

### Countries Dataset

```text
Countries.csv
```

Contains country-related information and is used in the Countries Data Analysis project.

### Anime Dataset

```text
anime.xls
```

An Excel dataset used for practicing data loading and analysis with Pandas.

Pandas can read Excel files using:

```python
pd.read_excel("anime.xls")
```

---

# 📂 Repository Structure

```text
Pandas/
│
├── 1. Series.ipynb
├── 2. Data Frame.ipynb
├── 3. MissingData.ipynb
├── 4. MergingjoiningandConcatination.ipynb
├── 5. GroupBy_and_Aggregation.ipynb
├── 6. Pivot_Table.ipynb
├── 7. Operations.ipynb
│
├── FeatureExtraction_Project-01.ipynb
├── Countries_Project-02.ipynb
│
├── Countries.csv
├── anime.xls
│
├── .gitattributes
└── README.md
```

The structure reflects the notebooks and datasets currently present in the repository.

---

# 🔄 Data Analysis Workflow

A typical Pandas-based data analysis workflow looks like this:

```text
Dataset
   ↓
Load Data
   ↓
Understand Data
   ↓
Clean Data
   ↓
Handle Missing Values
   ↓
Transform Data
   ↓
Group & Aggregate
   ↓
Analyze Data
   ↓
Extract Insights
```

---

# 🛠️ Technologies Used

| Technology          | Purpose                        |
| ------------------- | ------------------------------ |
| 🐍 Python           | Programming language           |
| 🐼 Pandas           | Data manipulation and analysis |
| 🔢 NumPy            | Numerical computing            |
| 📓 Jupyter Notebook | Interactive development        |
| 📄 CSV              | Dataset format                 |
| 📊 Excel            | Dataset format                 |

---

# ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Monu-kumar-kushwaha/Pandas.git
```

### 2. Navigate to the Project

```bash
cd Pandas
```

### 3. Install Pandas

```bash
pip install pandas
```

For the complete notebook environment:

```bash
pip install pandas numpy jupyter openpyxl
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

Open any `.ipynb` file and run the cells.

---

# 💻 Basic Pandas Example

```python
import pandas as pd

# Create a DataFrame
data = {
    "Name": ["Monu", "Rahul", "Amit"],
    "Marks": [85, 90, 78]
}

df = pd.DataFrame(data)

# Display data
print(df)

# Display statistics
print(df["Marks"].mean())

# Sort data
print(df.sort_values("Marks", ascending=False))
```

---

# 🎯 Learning Objectives

After completing this repository, you should be able to:

* Understand Pandas Series
* Understand Pandas DataFrames
* Load CSV and Excel datasets
* Select and filter data
* Handle missing values
* Merge multiple DataFrames
* Join datasets
* Concatenate DataFrames
* Group and aggregate data
* Create pivot tables
* Apply functions to data
* Sort and rank data
* Perform feature extraction
* Analyze real-world datasets
* Prepare data for Machine Learning

---

# 🌍 Real-World Applications

Pandas is widely used in:

* 📊 Data Science
* 📈 Data Analytics
* 🤖 Machine Learning
* 💼 Business Intelligence
* 💰 Finance
* 🏥 Healthcare
* 🛒 E-Commerce
* 🏏 Sports Analytics
* 🔬 Research
* 📉 Statistical Analysis

### Example

A company can use Pandas to analyze sales data:

```text
Sales Dataset
     ↓
Clean Data
     ↓
Group by Product
     ↓
Calculate Total Sales
     ↓
Find Best-Selling Product
     ↓
Business Decision
```

---

# 📈 Skills Demonstrated

This repository demonstrates practical skills in:

* Python Programming
* Pandas
* Data Manipulation
* Data Cleaning
* Data Analysis
* Feature Extraction
* Dataset Management
* Exploratory Data Analysis
* Statistical Operations
* Machine Learning Data Preparation

---

# 🔮 Future Improvements

Possible future additions include:

* [ ] Advanced Data Cleaning
* [ ] More Feature Engineering
* [ ] Exploratory Data Analysis projects
* [ ] Time-Series Data Analysis
* [ ] Large Dataset Analysis
* [ ] More real-world datasets
* [ ] Pandas + Matplotlib projects
* [ ] Pandas + Seaborn projects
* [ ] Machine Learning preprocessing projects
* [ ] Advanced data transformation

---

# ⭐ Why This Repository?

This repository provides a **hands-on approach to learning Pandas**.

Instead of learning Pandas only through theory, the notebooks allow you to practice:

* Data manipulation
* Data cleaning
* Data transformation
* Data aggregation
* Dataset combination
* Real-world data analysis

It is useful for **Python beginners, Data Science students, Data Analysts, and Machine Learning learners**.

---

# 👨‍💻 Author

**Monu Kumar Kushwaha**

GitHub:
https://github.com/Monu-kumar-kushwaha

---

# ⭐ Support

If you find this repository useful, consider giving it a ⭐ on GitHub.

Your support helps encourage more Data Science and Machine Learning projects.

---

## 📄 License

This repository is created primarily for **educational and learning purposes**.
