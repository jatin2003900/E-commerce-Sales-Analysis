# 🛒 E-Commerce Sales Analysis (EDA + SQL)

## 📌 Overview
This project focuses on analyzing e-commerce sales data to uncover meaningful business insights that can help improve sales performance, customer targeting, and strategic decision-making. The analysis combines **SQL for structured data querying** and **Python for data cleaning, exploratory data analysis (EDA), and visualization**.

The dataset is sourced from Kaggle and downloaded programmatically using the **Kaggle API**, ensuring reproducibility and automation.

---

## 🎯 Objectives
- Analyze e-commerce sales data to understand revenue trends and customer behavior  
- Perform data cleaning and preprocessing on raw sales data  
- Use SQL queries to extract structured insights from the dataset  
- Conduct exploratory data analysis (EDA) to identify patterns and trends  
- Generate actionable business insights from the analysis  

---

## 📂 Dataset
- **Source:** Kaggle (E-Commerce Sales Dataset)  
- **Format:** CSV  
- **Description:**  
  The dataset includes information related to orders, customers, products, quantities, prices, and timestamps.

---

## 🛠 Tools & Technologies
- **Python** – Core language for data analysis  
- **Pandas & NumPy** – Data cleaning, preprocessing, and manipulation  
- **SQL** – Querying and aggregating sales data  
- **SQLAlchemy** – Database connection and SQL execution  
- **Kaggle API** – Automated dataset download  
- **Jupyter Notebook** – Interactive analysis and visualization  

---

## 🔄 Project Workflow

### 1️⃣ Data Extraction
- Downloaded the dataset using the Kaggle API

### 2️⃣ Data Cleaning & Preprocessing
- Handled missing values and inconsistent records  
- Converted data types for accurate analysis  
- Removed duplicates and invalid entries  

### 3️⃣ SQL Analysis
- Performed aggregations and filtering using SQL queries  
- Extracted insights such as total sales, category-wise performance, and customer-level metrics  

### 4️⃣ Exploratory Data Analysis (EDA)
- Analyzed sales distribution and revenue trends  
- Studied customer purchasing behavior  
- Visualized insights using plots and charts  

### 5️⃣ Insights & Reporting
- Translated analytical results into meaningful business insights  

---

## 🧮 Sample SQL Queries

```sql
-- Total revenue by product category
SELECT category, SUM(quantity * price) AS total_revenue
FROM sales
GROUP BY category
ORDER BY total_revenue DESC;
