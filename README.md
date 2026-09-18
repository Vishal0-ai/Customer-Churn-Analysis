# 📊 Churn Data Analysis

An end-to-end **Customer Churn Data Analysis project** that demonstrates how raw and inconsistent customer data can be transformed into clean, structured data and meaningful business insights.

The project follows a complete analytics workflow using **Excel, Python, Pandas, MySQL, SQL, and Power BI**.

---

## 📌 Project Overview

The objective of this project is to analyze customer churn and identify patterns related to **customer retention, customer behaviour, and churn**.

The project covers the complete journey from **dirty raw data to an interactive Power BI dashboard**.

---

## 🔄 Project Workflow

```text
Excel (Dirty Churn Data)
          ↓
Python (Pandas)
          ↓
Data Cleaning
          ↓
Feature Engineering
          ↓
Export Clean Data
          ↓
MySQL Database
          ↓
SQL Analysis
          ↓
Power BI Dashboard
```

---

## 🎯 Project Objectives

- Clean and preprocess raw churn data
- Identify and handle data-quality issues
- Perform feature engineering
- Export clean and analysis-ready data
- Store the cleaned data in MySQL
- Use SQL to answer business-related questions
- Analyze customer churn patterns
- Build an interactive Power BI dashboard
- Present meaningful business insights

---

## 📂 Dataset

The project starts with a dirty customer churn dataset stored in Excel.

The raw dataset may contain issues such as:

- Missing values
- Duplicate records
- Incorrect data types
- Inconsistent categorical values
- Formatting issues
- Invalid or inconsistent entries

The dataset is loaded into Python using Pandas for inspection and cleaning.

---

## 🐍 Python & Pandas

Python and Pandas are used for data cleaning, preprocessing, and feature engineering.

### Key Activities

- Load Excel data
- Inspect the dataset
- Check missing values
- Identify duplicate records
- Check data types
- Handle inconsistent values
- Transform columns
- Create new features
- Validate the cleaned dataset

### Example

```python
import pandas as pd

df = pd.read_excel("churn_data.xlsx")

print(df.head())
print(df.info())
print(df.isnull().sum())
```

---

## 🧹 Data Cleaning

The raw churn dataset is cleaned before being used for further analysis.

### Cleaning Process

```text
Raw Data
   ↓
Data Inspection
   ↓
Missing Value Handling
   ↓
Duplicate Removal
   ↓
Data Type Correction
   ↓
Categorical Value Standardization
   ↓
Data Validation
   ↓
Clean Dataset
```

### Cleaning Techniques

- Handling missing values
- Removing duplicate records
- Correcting data types
- Standardizing categorical values
- Handling inconsistent entries
- Removing unnecessary columns
- Validating cleaned data

---

## ⚙️ Feature Engineering

Feature engineering is used to create meaningful features from the existing dataset.

Examples include:

- Customer tenure groups
- Age groups
- Customer segments
- Churn indicators
- Purchase or usage categories
- Other derived analytical features

Feature engineering helps make the data more useful for business analysis and customer segmentation.

---

## 💾 Export Clean Data

After completing data cleaning and feature engineering, the final dataset is exported as a clean and analysis-ready file.

```text
Dirty Excel Data
       ↓
Python + Pandas
       ↓
Clean & Feature-Engineered Data
       ↓
Export Clean Data
```

The cleaned data is then imported into MySQL for SQL-based analysis.

---

## 🗄️ MySQL Database

The cleaned dataset is stored in a MySQL database.

### Database Workflow

```text
Cleaned Dataset
      ↓
MySQL Table
      ↓
SQL Queries
      ↓
Business Analysis
      ↓
Business Insights
```

MySQL provides a structured environment for querying and analyzing the cleaned customer data.

---

## 🔎 SQL Analysis

SQL is used to answer business-related questions and extract insights from the cleaned data.

### Business Questions

- What is the total number of customers?
- How many customers have churned?
- What is the overall churn rate?
- Which customer segments have higher churn?
- How does churn vary by age group?
- How does customer tenure relate to churn?
- Which categories have the highest churn?
- How does churn differ between different customer groups?
- Which customer characteristics are associated with higher churn?

### Example SQL Query

```sql
SELECT
    Churn,
    COUNT(*) AS Customer_Count
FROM churn_data
GROUP BY Churn;
```

---

## 📊 Power BI Dashboard

The analyzed data is used to create an interactive Customer Churn Dashboard using Power BI.

### Dashboard Components

- Total Customers
- Churned Customers
- Churn Rate
- Customer Segmentation
- Churn by Age Group
- Churn by Tenure
- Churn by Category
- Customer Behaviour Analysis
- Interactive Filters
- Interactive Slicers
- KPI Cards
- Charts and Visualizations

The dashboard provides an easy way to explore customer churn and compare different customer segments.

---

## 📈 Dashboard Workflow

```text
MySQL Database
      ↓
Power BI
      ↓
Data Connection
      ↓
Data Modeling
      ↓
DAX Measures
      ↓
Visualizations
      ↓
Interactive Churn Dashboard
```

---

## 💡 Key Insights

The analysis is designed to identify patterns such as:

- Overall customer churn
- Customer segments with higher churn
- Differences in churn across demographic groups
- Relationship between customer tenure and churn
- Churn patterns across different services or categories
- Customer characteristics associated with churn

> **Note:** Specific numerical insights can be added here after completing the final SQL analysis and Power BI dashboard.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Microsoft Excel | Raw / dirty dataset |
| Python | Data processing |
| Pandas | Data cleaning and transformation |
| MySQL | Database storage |
| SQL | Business analysis |
| Power BI | Dashboard and visualization |
| DAX | KPI and analytical calculations |

---

## 📂 Project Structure

```text
Churn-Data-Analysis/
│
├── data/
│   ├── dirty_churn_data.xlsx
│   └── cleaned_churn_data.csv
│
├── python/
│   └── churn_data_cleaning.ipynb
│
├── sql/
│   └── churn_analysis.sql
│
├── powerbi/
│   └── churn_dashboard.pbix
│
├── images/
│   └── churn_dashboard.png
│
└── README.md
```

---

## ▶️ How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/Vishal0-ai/Churn-Data-Analysis.git
```

### 2. Navigate to the Repository

```bash
cd Churn-Data-Analysis
```

### 3. Install Python Libraries

```bash
pip install pandas openpyxl jupyter
```

### 4. Run the Python Notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open the churn data-cleaning notebook and run the cells sequentially.

### 5. Create MySQL Database

Create a MySQL database:

```sql
CREATE DATABASE churn_analysis;

USE churn_analysis;
```

Import the cleaned dataset into the required MySQL table.

### 6. Run SQL Analysis

Open:

```text
sql/churn_analysis.sql
```

Execute the queries to perform the business analysis.

### 7. Open Power BI Dashboard

Open:

```text
powerbi/churn_dashboard.pbix
```

Connect the dashboard to the MySQL database if required and refresh the data.

---

## 🎯 Skills Demonstrated

- Data Analytics
- Data Cleaning
- Data Preprocessing
- Feature Engineering
- Exploratory Data Analysis
- Business Analysis
- Customer Churn Analysis
- Python
- Pandas
- Jupyter Notebook
- Excel Data Processing
- SQL
  - SELECT
  - WHERE
  - GROUP BY
  - ORDER BY
  - Aggregate Functions
  - CASE Statements
  - JOINs
  - Subqueries
- MySQL
- Business Intelligence
- Power BI
- Data Modeling
- DAX
- KPI Development
- Data Visualization
- Dashboard Development

---

## 🔗 End-to-End Analytics Pipeline

```text
              RAW DATA
                  ↓
       Excel Dirty Churn Data
                  ↓
            Python + Pandas
                  ↓
           Data Cleaning
                  ↓
        Feature Engineering
                  ↓
          Cleaned Dataset
                  ↓
             MySQL DB
                  ↓
            SQL Analysis
                  ↓
         Business Insights
                  ↓
             Power BI
                  ↓
       Interactive Dashboard
```

---

## 📌 Project Outcome

This project demonstrates an end-to-end approach to Customer Churn Analytics.

The workflow combines:

- **Python + Pandas** for data cleaning and feature engineering
- **MySQL + SQL** for business-related analysis
- **Power BI** for interactive visualization and dashboard development

The final solution transforms dirty customer data into clean, structured, and meaningful business insights.

---

## 🚀 Future Improvements

- Add advanced customer segmentation
- Perform deeper churn analysis
- Add more DAX measures
- Add customer lifetime value analysis
- Add interactive drill-through pages
- Add churn prediction using Machine Learning
- Automate the data pipeline
- Connect Power BI directly to the production database

---

## 👤 Author

**Vishal Yadav**

*Aspiring Data Analyst | Python | Pandas | SQL | MySQL | Power BI*

I am building practical end-to-end projects to strengthen my skills in Data Analytics, Business Intelligence, Python, SQL, and Power BI.

⭐ If you find this project useful, consider starring the repository.
