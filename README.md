# Adventure work challenge 

## 📌 Project Overview

The **Adventure work challenge** is a complete business intelligence project developed using ** Power Query, and excel**.
This project focuses on analyzing sales performance, profitability, employee performance, reseller contributions, and regional trends using the Adventure Park dataset.

The project transforms raw transactional data into interactive dashboards and meaningful business insights for decision-making.

---

# 🚀 Objectives

* Analyze overall sales and profitability
* Identify top-performing products and regions
* Track employee sales performance
* Compare target vs actual sales
* Analyze reseller contributions
* Discover monthly and yearly sales trends
* Build interactive dashboards for business reporting

---

# 🛠️ Tools & Technologies Used

| Tool               | Purpose                        |
| ------------------ | ------------------------------ |
| Microsoft Power BI | Dashboard Development          |
| Power Query        | Data Cleaning & Transformation |
| DAX                | KPI & Measure Calculations     |
| CSV Files          | Raw Data Source                |
| Microsoft Excel    | Data Handling                  |

---

# 📂 Dataset Information

The dataset contains multiple business-related tables:

| Table Name         | Description                          |
| ------------------ | ------------------------------------ |
| Product            | Product category and pricing details |
| Sales              | Main transactional sales data        |
| Reseller           | Customer/reseller information        |
| Region             | Regional and country information     |
| Salesperson        | Employee details                     |
| Salesperson Region | Employee-region mapping              |
| Targets            | Monthly sales targets                |

---

# 🔄 Data Preprocessing

Data preprocessing was performed using **Power Query Editor**.

## Steps Performed

* Removed unnecessary columns
* Cleaned currency symbols
* Standardized data types
* Handled null values
* Merged multiple tables
* Created calculated columns
* Built relationships between tables
* Created Month Name column for trend analysis

## Feature Engineering

Created:

* Total Profit
* Profit Margin %
* Monthly Analysis Columns
* Target Achievement %

---

# 🔗 Data Modeling

Relationships were created between:

* Sales ↔ Product
* Sales ↔ Reseller
* Sales ↔ Region
* Sales ↔ Salesperson
* Targets ↔ Salesperson

---

# 📊 Key KPIs

## Sales KPIs

* Total Revenue
* Total Cost
* Total Profit
* Profit Margin %
* Total Orders
* Total Quantity Sold
* Average Order Value

## Employee KPIs

* Employee Sales
* Target Achievement %
* Best Performing Employee

## Product KPIs

* Top Category
* Most Profitable Product
* Low Demand Products

## Regional KPIs

* Best Performing Region
* Country-wise Revenue
* State-wise Sales

---

# 📈 Dashboard Pages

## 1️⃣ Executive Overview Dashboard

Includes:

* Revenue Overview
* Profit Overview
* Monthly Sales Trend
* Top Categories

### Visuals Used

* KPI Cards
* Line Charts
* Donut Charts
* Bar Charts

---

## 2️⃣ Sales Analysis Dashboard

Includes:

* Region-wise Sales
* Country-wise Revenue
* Profit Analysis
* Sales Trends

### Visuals Used

* Map Visual
* Area Chart
* Clustered Bar Chart

# 🧮 DAX Measures Used

```DAX
Total Revenue = SUM(Sales[Sales])

Total Cost = SUM(Sales[Cost])

Total Profit = [Total Revenue] - [Total Cost]

Profit Margin % =
DIVIDE([Total Profit],[Total Revenue],0)

Total Orders =
DISTINCTCOUNT(Sales[Sales Order Number])

Average Order Value =
DIVIDE([Total Revenue],[Total Orders],0)

Target Achievement % =
DIVIDE([Total Revenue],SUM(Targets[Target]),0)
```

---

# 📌 Business Insights

* Certain product categories generate maximum revenue.
* Some regions contribute lower sales and need improvement.
* A few salespersons contribute major business revenue.
* Profit margins vary significantly across product categories.
* Seasonal sales trends impact overall performance.

---

# 💡 Recommendations

* Focus marketing on high-performing regions
* Improve sales strategies in low-performing areas
* Reward top-performing employees
* Promote high-profit products aggressively
* Increase reseller partnerships in profitable cities

---

# ✅ Project Outcome

This project successfully transformed raw business data into a structured analytical model and interactive dashboard solution that supports:

* Sales Analysis
* Profitability Analysis
* Employee Performance Tracking
* Regional Performance Evaluation
* Business Decision-Making

