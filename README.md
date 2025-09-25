# Data Analyst Internship — Task 4: Dashboard Design

## Objective
Design an interactive dashboard in **Power BI** for business stakeholders.  
The dashboard helps track **Sales, Profit, and Growth KPIs** to support decision-making.

---

## Dataset
- File: `sales_financial_dataset.csv`
- Rows: 1,200 (synthetic Superstore-like data)
- Columns:
  - OrderID, OrderDate, Region, Category, Sub-Category, Product, Quantity, Price, Sales, Discount, Profit

---

## Power BI Dashboard Deliverables
### KPIs (DAX Measures)
- Total Sales = `SUM(Sales)`  
- Total Profit = `SUM(Profit)`  
- Total Orders = `DISTINCTCOUNT(OrderID)`  
- Avg Order Value = `Total Sales / Total Orders`  
- Profit Margin % = `Total Profit / Total Sales`  
- Sales YoY % (Year-over-Year growth)

### Dashboard Pages
1. **Overview**
   - KPI Cards (Sales, Profit, Orders, AOV, Margin)
   - Monthly Sales Trend (line chart)
   - Sales by Region (bar chart)
   - Slicers for Region, Category, Year

2. **Sales Deep Dive**
   - Sales by Category over time (stacked column)
   - Matrix with Product-level details (Sales, Quantity, Profit)
   - Top 10 Products by Sales (bar chart)
   - Slicers for Sub-Category, Product

3. **Profit & Growth**
   - Profit Trend (line chart)
   - Sales YoY % (KPI visual)
   - Waterfall Chart for YoY change

---

## Outcome
- Learn how to build dashboards with KPIs, filters, and interactivity.
- Identify trends in sales, profit, and product performance.
- Provide actionable insights for business decisions.

---

## Files Included
- `sales_financial_dataset.csv` → Input dataset  
- `Dashboard_Task4.pbix` → Power BI file (to be created by importing dataset and DAX measures)  
- `dashboard_summary_expanded.pptx` → PowerPoint summary with design guide and insights  
- `README.md` → This file

---

## Instructions to Run
1. Open **Power BI Desktop**.  
2. Load the dataset: *Get Data → Text/CSV → sales_financial_dataset.csv*.  
3. Create DAX measures (from above).  
4. Build dashboard pages as described.  
5. Save as `Dashboard_Task4.pbix`.  

---

## Sample Insights (Synthetic Data)
- East & West regions generate the most sales.  
- Technology category shows strong revenue growth.  
- Discounts have mixed impact: sometimes boosting sales but reducing margin.  
- Chairs and Computers are among top-selling products.

---

**Author:** Elevate Labs Internship — Task 4 Submission
