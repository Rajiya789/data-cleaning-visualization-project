# 📊 Data Cleaning & Visualization Project

## 📌 Project Overview

This project focuses on cleaning, processing, analyzing, and visualizing a raw sales dataset using Python.

The main objective is to demonstrate practical data preprocessing and exploratory data analysis techniques, including handling missing values, removing duplicate records, identifying and handling outliers, and creating meaningful visualizations to discover patterns and insights from the data.

---

## 🎯 Project Objectives

The key objectives of this project are:

* Clean and preprocess raw sales data
* Identify and handle missing values
* Detect and remove duplicate records
* Identify and handle outliers
* Correct inconsistent data values
* Perform exploratory data analysis (EDA)
* Create meaningful data visualizations
* Identify important patterns and trends
* Present findings through data storytelling

---

## 🛠️ Technologies & Libraries Used

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Google Colab** – Development environment

---

## 📂 Dataset

The project uses a raw sales dataset containing information about:

* Order Date
* Customer Name
* Product
* Category
* Region
* Quantity
* Unit Price
* Sales
* Profit

The raw dataset intentionally contains data-quality issues such as missing values, duplicate records, inconsistent region names, and outliers to demonstrate the data-cleaning process.

---

## 🧹 Data Cleaning Process

The following preprocessing steps were performed:

### 1. Missing Values

Missing values were identified using Pandas.

```python
df.isnull().sum()
```

Numerical missing values were handled using the median, while categorical missing values were handled using the mode.

### 2. Duplicate Records

Duplicate records were identified and removed.

```python
df.duplicated().sum()
```

```python
df = df.drop_duplicates()
```

### 3. Inconsistent Values

Inconsistent categorical values such as different capitalization and extra spaces were standardized.

For example:

```text
south
South
SOUTH
```

were standardized into a consistent format.

### 4. Outlier Detection

Boxplots and the Interquartile Range (IQR) method were used to identify extreme values.

The IQR method was used to handle unusually high values in numerical columns such as:

* Quantity
* Sales
* Profit

### 5. Data Type Checking

The data types of the columns were inspected and corrected where necessary.

---

## 📊 Exploratory Data Analysis

After cleaning the dataset, exploratory data analysis was performed to understand:

* Product distribution
* Category distribution
* Regional sales
* Sales and profit patterns
* Numerical variable distributions
* Relationships between numerical variables

---

## 📈 Data Visualizations

The following visualizations were created:

### 📊 Bar Chart

Used to understand the distribution of products or categories.

### 📉 Histogram

Used to understand the distribution of numerical variables such as sales and profit.

### 📦 Box Plot

Used to detect and understand outliers.

### 🥧 Pie Chart

Used to visualize the proportion of different categories or regions.

### 🔵 Scatter Plot

Used to analyze relationships between numerical variables such as sales and profit.

### 🔥 Correlation Heatmap

Used to identify relationships between numerical variables.

---

## 🔍 Key Insights

The analysis helps identify:

* The distribution of sales across different products and categories
* Regional differences in sales performance
* The relationship between sales and profit
* The distribution of quantities sold
* Unusual values and potential outliers
* Relationships between numerical variables

The exact insights are based on the results generated during the exploratory data analysis.

---

## 📁 Project Structure

```text
data-cleaning-visualization-project/
│
├── raw_sales_data.csv
├── cleaned_sales_data.csv
├── Data_Cleaning_Visualization.ipynb
├── README.md
└── visualizations/
```

---

## ▶️ How to Run the Project

### Option 1: Google Colab

1. Open Google Colab.
2. Upload the `Data_Cleaning_Visualization.ipynb` notebook.
3. Upload `raw_sales_data.csv`.
4. Run the notebook cells sequentially.
5. View the cleaning process, analysis, and visualizations.

### Option 2: Local Python Environment

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

Then open the Jupyter Notebook and run the cells.

---

## 📌 Expected Outcome

This project provides practical experience in:

* Data preprocessing
* Data cleaning
* Exploratory data analysis
* Statistical analysis
* Data visualization
* Identifying patterns and trends
* Data storytelling

---

## 🎓 Learning Outcome

Through this project, I gained hands-on experience in using Python libraries such as Pandas, NumPy, Matplotlib, and Seaborn to transform raw data into clean, meaningful, and visually understandable information.

---

## 👩‍💻 Author

**Rajiya**

Data Analysis & Visualization Project
