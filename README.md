# 📈 AdventureWorks Sales Analysis (Power BI Advanced Project)
***Final Level to a beginner Power BI Project - self working***

### Dashboard Link : [https://app.powerbi.com/groups/me/reports/384d017e-e935-44dc-9e7d-1626c1a36de1/ReportSection](https://app.powerbi.com/view?r=eyJrIjoiYjk4ZGY0ODEtYzA5NC00NjRjLTkxNzEtMDcwZjIzNWI4NDcxIiwidCI6IjE0YmYyODYxLWFhNDctNGQ1Yi1iOTAxLWU1ZGJjMDEyYjgxNSJ9)

This repository presents an **advanced-level Power BI project** built using the AdventureWorks dataset. The focus of this project is on **advanced DAX time intelligence**, performance analysis, and profitability metrics. It leverages dynamic calculations to assess historical trends such as **Previous Year, Month, YTD, QTD, MTD, YoY, QoQ, and MoM performance**, providing a comprehensive view of business insights over time.

---

## 📂 Files Included

- 🟨 **Adventure Works Sales [Advanced].pbix**  
  Power BI file containing all advanced DAX measures, time intelligence, and report visuals.

- 📄 **Adventure Works Sales [Advanced] Problem Statement.docx**  
  Document describing the problem statement, DAX implementations, solution challenges, and key insights.

- 📊 **AdventureWorks_Sale_3.xlsx**  
  Excel source dataset containing sales transactions, product, customer, date, and territory data.

---

## ⚙️ Project Highlights

### 🧠 Advanced DAX Calculations

- **Category-Level Filtering:**
  - Total sales for the *Accessories* category using `CALCULATE()` with `FILTER()` logic.

- **Time Intelligence Measures:**
  - `Previous Year Sales` using `PREVIOUSYEAR()` and `SAMEPERIODLASTYEAR()`
  - `Previous Month Sales` using `PARALLELPERIOD()`

- **Rolling Window Metrics:**
  - `Quantity Sold in Last 3 Months` (custom logic to sum over trailing months)
  - `Profit for Last 6 Months` (manual sum with dynamic date filters)

- **Cumulative Aggregations:**
  - `YTD` (Year-to-Date)
  - `QTD` (Quarter-to-Date)
  - `MTD` (Month-to-Date)

- **Growth Metrics:**
  - `YoY` – Year-over-Year
  - `QoQ` – Quarter-over-Quarter
  - `MoM` – Month-over-Month  
  *(All created via Power BI’s Quick Measures for accurate time-based comparisons)*

> ⚠️ Note: Corrected implementations of trailing period aggregations were applied. Many common DAX templates like `DATEADD()` or `SAMEPERIODLASTYEAR()` were tested and refined to ensure logic matches the actual business requirement (e.g., total of the last 3 months, not just a specific one).

---

## 📊 Visualization Dashboard

- Custom visuals showcasing all calculated measures.
- **Matrix tables**, **line and bar charts**, and **comparison visuals** across date hierarchies.
- Clear layout for users to explore:
  - Monthly & quarterly trends
  - Profit growth vs. cost over time
  - Historical comparisons (YoY, MoM, QoQ)

---

## 🧹 Data Modeling & Preparation

- Reused cleaned data model from the Intermediate project.
- Validated and preserved **star schema** structure:
  - Key relationships established between `Sales`, `Date`, `Products`, and other dimension tables.
- Measures organized into a dedicated **"Questions"** table for clarity and performance.

---

## 🧠 What You’ll Learn

- Writing and debugging **custom time-based DAX measures**
- Applying `CALCULATE()` with dynamic filters for KPIs
- Understanding the nuance between `SUM()` vs. `SUMX()` in context
- Visualizing performance metrics over time using effective design patterns
- Identifying and fixing common pitfalls in rolling window DAX logic

---

## 🛠 Tools & Technologies

- **Power BI Desktop**
- **Power Query Editor**
- **DAX (Data Analysis Expressions)**
- **Excel Workbook (.xlsx)**

---

## 🏷 Tags

`Power BI` `Advanced DAX` `Time Intelligence` `Profitability Metrics`  
`Sales Analytics` `YoY MoM QTD MTD YTD` `Rolling Aggregations` `AdventureWorks`

---

## 👤 Author

**Bidarth Kr. Singh**

## 📌 Credits

        This project was created by Bidarth Kr. Singh and is distributed under the "Apache License" license.

---

# Snapshot of Dashboard (Power BI Service)

![Image](https://github.com/user-attachments/assets/03a143c2-e2cb-48a8-8cd7-1183642fc3ea)
