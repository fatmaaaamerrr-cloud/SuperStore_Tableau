# 📊 Superstore Sales & Profitability Dashboard (Tableau)

Interactive Tableau dashboards that analyze **Superstore** sales performance, profitability, customers, and products. The data is modeled in a **Data Warehouse (Star Schema)** and connected directly to Tableau.

## 🎯 Project Objective
Help management understand where the business makes money and where it loses it, by answering:
- How are sales and profit trending over time?
- Which regions, states, and customer segments drive profit?
- Which products and sub-categories are top performers, and which are loss makers?
- How do discounts affect sales and profitability?

## 🗄️ Data Model
Data comes from a `Superstore_DW` warehouse (`gold` schema) built as a **Star Schema**:

| Table | Description |
|---|---|
| `fact_sales` | Sales, Profit, Quantity, Discount |
| `dim_customer` | Customer ID, Name, Segment |
| `dim_product` | Product ID/Name, Category, Sub-Category |
| `dim_location` | Country, Region, State, City, Postal Code |
| `dim_order` | Order ID, Order Date, Ship Date |
| `dim_ship_mode` | Shipping mode |
| `dim_date` | Calendar year, quarter, month, day |

Also uses a reporting view: `vw_fact_sales_report`.

## 📈 Dashboards

### 1. Executive Overview
High-level KPIs (Total Sales, Total Profit, Profit Margin, Total Orders), Sales & Profit trend, and profit by location.

### 2. Product Performance & Portfolio
Top 10 products, loss-making products, performance by category and sub-category, and Sales Volume vs. Profitability.

### 3. Customer & Sales Behavior
Customer segment analysis, Top 10 customers, and the impact of discount levels on sales and profit.

## ⚙️ Key Features
- **Dynamic parameters**: switch the time level (Year / Quarter / Month) and the geography level (Country / State) on the fly.
- **Calculated fields**: Profit Margin, Cost, Total Orders (distinct count), Discount Bucket.
- **Discount segmentation**: No Discount, Low (≤20%), Medium (21–40%), High (>40%).
- **Visuals**: KPI cards, trend lines, bar charts, scatter plots, and geographic maps.

## 🛠️ Tools & Skills
- Tableau Desktop
- Data Warehousing (Star Schema, Fact & Dimension tables)
- SQL (gold layer / reporting view)
- Data Visualization & Dashboard Design
- Calculated Fields & Parameters

## 📁 Repository Structure
