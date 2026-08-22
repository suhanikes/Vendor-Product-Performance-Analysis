# Vendor & Product Performance Analysis

## 📌 Project Overview

This project analyzes vendor and product performance to identify opportunities for improving **sales performance, procurement efficiency, profitability, and inventory management**.

The analysis combines **SQL, Python, Pandas, NumPy, statistical analysis, and Power BI** to transform raw vendor and product data into actionable business insights.

---

## 🎯 Business Objectives

The analysis focuses on answering the following questions:

- Which vendors and products contribute the most to sales and procurement spend?
- Which products combine high profit margins with meaningful sales volume?
- How concentrated is procurement across vendors?
- Which vendors have relatively low sales compared with their purchases?
- Which vendors contribute the most to estimated inventory exposure?
- How can vendor and product performance be improved?

---

## 📊 Dataset

- **10,692 records**
- **18 attributes**
- **128 vendors**
- **9,483 products**

Key fields include:

- Vendor Name
- Product Description
- Purchase Price
- Actual Price
- Purchase Quantity
- Purchase Dollars
- Sales Quantity
- Sales Dollars
- Gross Profit
- Profit Margin
- Stock Turnover
- Sales-to-Purchase Ratio

---

## 🛠️ Tools & Technologies

- **SQL** – Data extraction and querying
- **Python** – Data analysis and transformation
- **Pandas & NumPy** – Data manipulation and feature engineering
- **Matplotlib & Seaborn** – Exploratory data visualization
- **SciPy** – Statistical analysis
- **Power BI** – Interactive dashboard and business reporting

---

## 🔍 Analysis Performed

### 1. Data Cleaning & Quality Checks

Performed data-quality validation to identify:

- Missing values
- Duplicate records
- Negative gross profit
- Zero/negative sales
- Invalid purchase quantities

Loss-making records were retained where they represented genuine business conditions, while invalid records were excluded only where required for specific metric calculations.

### 2. Vendor Performance Analysis

Calculated and compared:

- Total purchase spend
- Total sales
- Gross profit
- Profit margin
- Purchase contribution
- Sales contribution
- Gross-profit contribution

The analysis showed that the **top 10 vendors accounted for 65.33% of total purchase spend and 65.01% of total sales**, highlighting significant vendor concentration.

### 3. Product Performance Analysis

Evaluated products based on:

- Sales
- Sales volume
- Gross profit
- Profit margin

Identified **10 opportunity products** using a combination of relatively low sales, high profit margin, and meaningful sales volume.

### 4. Inventory Exposure Analysis

Estimated potential inventory exposure using:

`Estimated Inventory Exposure = Unsold Quantity × Purchase Price`

This helped identify vendors with the largest estimated inventory exposure and potential slow-moving inventory.

---

## 📈 Key Business Insights

- Total sales were approximately **$1.35B**.
- Gross profit was approximately **$1.03B**.
- Overall profit margin was approximately **76.3%**.
- Procurement and sales were highly concentrated among the top vendors.
- Certain products showed **high margins despite relatively lower sales**, indicating potential opportunities for targeted commercial strategies.
- Vendor-level analysis identified areas of potential **slow-moving inventory and procurement inefficiency**.

---

## 📊 Power BI Dashboard

The project includes an interactive Power BI dashboard covering:

- Total Sales
- Total Purchase
- Gross Profit
- Profit Margin
- Estimated Inventory Exposure
- Top Vendors by Sales
- Top Products by Sales
- Vendor Procurement Concentration
- Vendors with Low Sales-to-Purchase Ratio

The dashboard converts the analytical findings into an executive-friendly view for monitoring **vendor performance, procurement concentration, profitability, and inventory risk**.

---

## 💡 Business Recommendations

Based on the analysis:

1. **Optimize procurement concentration** by monitoring dependence on high-contribution vendors.
2. **Prioritize high-margin product opportunities** through targeted sales and promotional strategies.
3. **Review low sales-to-purchase vendors** to identify potential overstocking and slow-moving inventory.
4. Use vendor and product KPIs regularly to support **data-driven procurement and inventory decisions**.

---

## 📁 Project Structure

```text
Vendor-Product-Performance-Analysis/
│
├── Vendor_Performance_Analysis.ipynb
├── inventory.db
├── PowerBI_Dashboard.pbix
└── README.md
