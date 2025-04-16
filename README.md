# 📊 Business Performance KPI Dashboard

## Table of Contents
- [Introduction](#Introduction)
- [Objective](#Objective)
- [Tools & Technologies](#Tools-&-Technologies)
- [Dataset](#Dataset)
- [Data Preparation (Python)](#Data-Preparation-(Python))
- [Dashboard Overview (Power BI)](#Dashboard-Overview-(Power-BI))
- [Business Insights](#Business-Insights)

## Introduction
This project is a complete end-to-end Business Intelligence solution, where raw sales data is transformed, cleaned, and analyzed to create an interactive **Business Performance KPI Dashboard** in Power BI. Python is used for data preparation, and the dashboard provides valuable insights into business trends and product performance.

## Objective

The goal of this project is to:
- Clean and preprocess sales data using **Python**
- Perform **exploratory data analysis** (EDA)
- Build a dynamic **KPI dashboard** in **Power BI**

## Tools & Technologies

| Tool          | Purpose                                  |
|---------------|------------------------------------------|
| Python        | Data cleaning and preprocessing          |
| Pandas        | Data manipulation                        |
| Power BI      | Dashboard and data visualization         |

## Dataset

- The dataset includes sales records such as:
  - InvoiceNo
  - CustomerID
  - Product information
  - Order date
  - Country
  - Unit price and quantity
- Source: [Kaggle/Excel/Online Retail dataset]

## Data Preparation (Python)

In the Python script (`Business_Performance_KPI_Dashboard.ipynb`):

1. **Loading the Dataset**:
   - Used `pandas` to load `.csv` files.
   - Checked for missing values and nulls.

2. **Data Cleaning**:
   - Removed duplicate records and canceled orders (negative quantities).
   - Converted columns to appropriate datatypes (e.g., datetime).

3. **Feature Engineering**:
   - Created `TotalPrice = UnitPrice * Quantity`
   - Filtered out non-valuable rows (e.g., null `CustomerID`, returns).

4. **Export**:
   - Cleaned dataset was saved as `.csv` for use in Power BI.


## Dashboard Overview (Power BI)

### Dashboard: Sales Performance

| Visualization                  | Insight Provided                                     |
|-------------------------------|------------------------------------------------------|
| 📆 Sales Trends (Year/Month)  | Tracks how sales change over time                   |
| 👥 Sales by Customer Type     | Compares regular customers and guests               |
| 🛍️ Top 10 Products            | Identifies best-performing products                 |
| 🌍 Sales by Country           | Shows geographical distribution of sales            |
| 📅 Sales by Month             | Reveals seasonal trends in sales                    |


## Business Insights

- Peak sales were observed during the holiday season.
- The company's revenue comes from the top 10 products.
- Some countries outperform others in sales, which is useful for geo-targeting.
