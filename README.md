# 📊 Business Insights 360 Dashboard

A Power BI dashboard delivering a 360-degree view of financial and sales performance across customers, products, and geographies. It enables stakeholders to monitor KPIs like Net Sales, Gross Margin, and Profitability — with intuitive visualizations and robust data modeling.

---

## 🧭 Overview

**Business Insights 360** includes two primary analytical modes:

- **Finance View**: Get a full P&L statement across any customer, product, or country dimension.
- **Sales View**: Evaluate performance over key metrics like Net Sales, Gross Margin %, and Customer/Product profitability.

---

## 💡 Key Features

### 📈 Finance View
- Profit & Loss Statement with Year-over-Year (YoY) change
- COGS breakdown including manufacturing, freight, and other costs
- Net Profit after operational expenses
- Gross Margin per Unit calculation
- Time-based trend analysis

### 💼 Sales View
- **Customer Performance**: Table with Net Sales, Gross Margin $, and GM%
- **Product Performance**: Segment-wise contribution and profitability
- **Performance Matrix**: Regional scatter plot (NS $ vs GM $)
- **Unit Economics**: Visualization of Net Sales breakdown and cost structures

---

## 📊 KPIs Tracked

- **Net Sales**: $3.74B
- **Gross Margin**: $1.42B (38.08%)
- **COGS**: $2.31B
- **Net Profit**: -$522M
- **Gross Margin/Unit**: $15.76

---

## 🌐 Top Performers

- **Customer**: Amazon ($496.88M NS, 36.78% GM%)
- **Product Segment**: Notebook ($1.58B NS, 39.03% GM%)
- **Region**: APAC ($1.92B NS)

---

## 🗂 Data Model

The dashboard is powered by a well-structured **star schema** data model. Below is a simplified overview:

### 📌 Star Schema Entities

- **Fact Tables**:
  - `fact_actuals_estimates`
  - `fact_forecast_monthly`
  - `post_invoice_deductions`
  - `manufacturing_cost`
  - `freight_cost`
  - `Operational_expense`

- **Dimension Tables**:
  - `dim_customer`
  - `dim_product`
  - `dim_market`
  - `dim_date`
  - `fiscal_year`

### 🔗 Relationships:
- One-to-many relationships from dimensions to facts
- Common join keys include `product_code`, `customer_code`, `fiscal_year`, and `date`

![Data Model Schema](./7c3b83fd-8297-4ae7-8715-3289429e33ac.png)

---

## 📂 Project Structure

📁 Business-Insights-360/
│
├── Finance.png # Finance View screenshot
├── Sales.png # Sales View screenshot
├── Homepage.png # Homepage for user navigation
├── DataModelling.png # Power BI data model diagram
└── README.md # This file
