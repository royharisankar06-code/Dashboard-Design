# Dashboard-Design
Design an interactive dashboard for business stakeholders.
Total Sales = SUM('sales_financial_dataset'[Sales])

Total Profit = SUM('sales_financial_dataset'[Profit])

Total Orders = DISTINCTCOUNT('sales_financial_dataset'[OrderID])

Average Order Value = DIVIDE([Total Sales], [Total Orders], 0)

Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)

Sales YoY % = 
VAR CurrentSales = [Total Sales]
VAR PriorSales = CALCULATE(
    [Total Sales],
    SAMEPERIODLASTYEAR('sales_financial_dataset'[OrderDate])
)
RETURN
IF(NOT(ISBLANK(PriorSales)), (CurrentSales - PriorSales) / ABS(PriorSales), BLANK())
