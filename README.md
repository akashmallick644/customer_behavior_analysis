# customer_behavior_analysis
Data Analytics project showcasing customer behavior analysis using Python, SQL and Power BI.
# 📊 Data Analytics Project

## Overview

This project demonstrates an end-to-end **data analytics workflow**, starting from raw data and progressing through data exploration, cleaning, SQL analysis, dashboard development, and presentation.

The project uses **Python, PostgreSQL, Power BI, and Gamma AI** to transform raw data into meaningful business insights and visualizations.

### Project Workflow

**Dataset → Python EDA → Data Cleaning → PostgreSQL SQL Analysis → Power BI Dashboard → Gamma AI Presentation**

---

## 📁 Dataset

The project starts with a raw dataset that is loaded and analyzed using Python.

The dataset is explored to understand:

* Data structure and column information
* Missing values
* Duplicate records
* Data types
* Numerical and categorical variables
* Trends and patterns
* Potential data quality issues

> **Dataset:** customer_shopping_behavior(1).csv

---

## 🛠️ Tools & Technologies

| Tool                     | Purpose                                 |
| ------------------------ | --------------------------------------- |
| **Python**               | Data loading, exploration, and cleaning |
| **Pandas**               | Data manipulation and preprocessing     |
| **NumPy**                | Numerical analysis                      |
| **Matplotlib / Seaborn** | Exploratory data visualization          |
| **PostgreSQL**           | SQL-based data analysis                 |
| **Power BI**             | Interactive dashboard development       |
| **Gamma AI**             | Presentation and storytelling           |
| **Jupyter Notebook**     | Python analysis environment             |

---

## 🔄 Project Steps

### 1. Data Loading

The dataset is imported into Python using **Pandas**.

```python
import pandas as pd

df = pd.read_csv("dataset.csv")

df.head()
```

Initial checks are performed to understand the dataset structure and identify potential issues.

---

### 2. Exploratory Data Analysis (EDA)

EDA is performed to identify patterns, trends, relationships, and anomalies within the data.

Key activities include:

* Dataset overview
* Descriptive statistics
* Missing-value analysis
* Duplicate detection
* Distribution analysis
* Correlation analysis
* Univariate and bivariate analysis
* Data visualization

Example:

```python
df.info()
df.describe()
df.isnull().sum()
df.duplicated().sum()
```

---

### 3. Data Cleaning

The raw dataset is cleaned and prepared for further analysis.

The cleaning process includes:

* Handling missing values
* Removing duplicate records
* Correcting data types
* Standardizing column names
* Handling inconsistent values
* Removing unnecessary columns
* Creating useful derived columns where required

The cleaned dataset is then prepared for SQL analysis and visualization.

---

### 4. SQL Analysis with PostgreSQL

The cleaned data is loaded into **PostgreSQL** for structured querying and business analysis.

SQL queries are used to answer analytical questions such as:

* What are the overall trends?
* Which categories/products perform best?
* What are the top-performing segments?
* How does performance change over time?
* What are the key business metrics?
* Are there noticeable patterns across different categories?

Example:

```sql
SELECT
    category,
    SUM(sales) AS total_sales
FROM sales_data
GROUP BY category
ORDER BY total_sales DESC;
```

The SQL analysis helps convert the cleaned dataset into meaningful business insights.

---

## 📊 Power BI Dashboard

The analyzed data is used to create an interactive **Power BI dashboard**.

### Dashboard Features

The dashboard includes:

* KPI cards
* Interactive charts
* Trend analysis
* Category/segment comparisons
* Filters and slicers
* Key performance indicators
* Business insights

## 🖥️ Presentation

A presentation was created using **Gamma AI** to communicate the project's findings in a concise and visually engaging format.

The presentation covers:

* Business problem
* Dataset overview
* Data preparation
* EDA findings
* SQL analysis
* Power BI dashboard
* Key insights
* Final conclusions



### 2. Install Required Python Libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Run the Python Analysis

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Then open the project notebook and run the cells sequentially.

### 4. PostgreSQL Setup

Create a PostgreSQL database and import the cleaned dataset.

Update the database connection details in the SQL/Python configuration as required.

Example:

```text
Host: localhost
Port: 5432
Database: analytics_db
Username: postgres
```

Run the SQL queries provided in the `sql/` folder.

### 5. Power BI

Open the Power BI `.pbix` file and refresh the data connection if required.

---

## 📂 Project Structure

```text
data-analytics-project/
│
├── data/
│   ├── raw/
│   └── cleaned/
│
├── notebooks/
│   └── data_analysis.ipynb
│
├── sql/
│   └── analysis_queries.sql
│
├── powerbi/
│   └── dashboard.pbix
│
├── presentation/
│   └── project_presentation.pdf
│
├── images/
│   └── dashboard.png
│
├── README.md
└── requirements.txt
```

---

## 🎯 Skills Demonstrated

* Data Cleaning & Preprocessing
* Exploratory Data Analysis
* Python & Pandas
* SQL & PostgreSQL
* Data Visualization
* Power BI Dashboard Development
* Business Intelligence
* Data Storytelling
* Presentation Development

---

## 👤 Author

Akash Mallick

**Data Analyst | Python | SQL | Power BI**

* GitHub: https://github.com/akashmallick644
* LinkedIn: www.linkedin.com/in/akash-mallick-8159b6223

---

## ⭐ Project Summary

This project demonstrates a complete **end-to-end data analytics pipeline**, from raw dataset exploration and cleaning to SQL analysis, interactive Power BI visualization, and business-focused presentation.

It showcases the ability to work with data across multiple tools and communicate analytical findings in a clear and business-friendly manner.
