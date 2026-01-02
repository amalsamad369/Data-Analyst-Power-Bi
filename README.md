Sales Analysis Dashboard

 Problem Statement

The purpose of this project is to analyze sales performance using historical sales data and present the findings through an interactive Power BI dashboard. The dashboard is designed to help business stakeholders understand overall sales trends, profitability, customer behavior, and regional performance.

By analyzing key sales indicators such as total sales, profit, quantity sold, and order volume, this dashboard enables decision-makers to identify high-performing products, underperforming regions, and seasonal trends. The insights derived from this analysis can support strategic planning, inventory management, and revenue optimization.

 Dataset Description

The dataset used for this project consists of sales transaction records collected over a specific time period. Each record represents an individual sales order and includes details such as order date, product category, customer segment, region, sales amount, profit, and quantity sold.

The dataset was provided in CSV/Excel format and was used strictly for learning and analytical purposes.

Tools and Technologies Used

Power BI Desktop

Power Query Editor

DAX (Data Analysis Expressions)

CSV / Excel Dataset

Steps Followed
Step 1: Data Loading

The sales dataset was imported into Power BI Desktop from a CSV/Excel file.

Step 2: Data Profiling

In Power Query Editor, data profiling options such as Column Distribution, Column Quality, and Column Profile were enabled to understand the structure and quality of the data. Profiling was performed on the entire dataset rather than the default sample rows.

Step 3: Data Cleaning

Missing values and inconsistencies were identified in numerical and categorical columns. Appropriate transformations were applied, including removal of invalid records and correction of data types.

Step 4: Data Transformation

Columns were formatted to ensure correct data types for dates, numerical values, and text fields. Derived fields were created where necessary to support analysis.

Step 5: Data Modeling

The data model was reviewed to ensure relationships were correctly defined and optimized for reporting.

Step 6: Report Design

A suitable report theme was applied for visual consistency. The report layout was designed to ensure clarity and ease of interpretation.

Step 7: Visual Filters (Slicers)

Slicers were added to allow dynamic filtering of the dashboard based on:

Region

Product Category

Customer Segment

Order Date

Step 8: KPI Creation

Card visuals were added to display key performance indicators such as:

Total Sales

Total Profit

Total Quantity Sold

Total Number of Orders

Step 9: Sales and Profit Analysis

Bar and column charts were created to analyze sales and profit across regions and product categories.

Step 10: Trend Analysis

Line charts were used to identify monthly and yearly sales trends and seasonal patterns.

Step 11: Product Performance Analysis

Visuals were added to highlight top-performing and underperforming products based on sales and profit metrics.

 DAX Calculations
Total Sales
Total Sales = SUM(Sales_Data[Sales])

Total Profit
Total Profit = SUM(Sales_Data[Profit])

Total Quantity Sold
Total Quantity Sold = SUM(Sales_Data[Quantity])

Total Orders
Total Orders = DISTINCTCOUNT(Sales_Data[Order ID])

Profit Margin Percentage
Profit Margin (%) =
DIVIDE([Total Profit], [Total Sales]) * 100

📸 Snapshot of Dashboard (Power BI Desktop)

![Power BI Dashboard](https://github.com/user-attachments/assets/f6573ab0-75d4-4a00-b4e3-55362135c55a)


📸 Individual Visual Snapshots

📌 Insert individual visual screenshots here (optional):

Sales by Region

Sales by Category

Monthly Sales Trend

Profit Analysis

(Example: /screenshots/sales_by_region.png)

🔍 Insights
[1] Overall Sales Performance

The dashboard provides a consolidated view of total sales, profit, quantity sold, and order volume. The analysis reveals noticeable variations in sales performance across different time periods, indicating the presence of seasonal demand patterns.

[2] Category-wise Analysis

Certain product categories contribute a significant portion of total sales revenue. However, some categories with high sales volume show comparatively lower profit margins, suggesting the need for pricing or cost optimization.

[3] Region-wise Analysis

Sales performance varies across regions. While some regions consistently perform well, others show lower sales and profit figures, highlighting potential opportunities for targeted marketing or expansion.

[4] Time-based Trends

Monthly and yearly trend analysis indicates clear seasonal peaks and slow periods. These insights can help businesses plan inventory, staffing, and promotional activities more effectively.

[5] Customer Segment Analysis

The analysis shows that a specific segment of customers contributes disproportionately to total revenue. Understanding this behavior can help in designing customer retention and loyalty strategies.

🚀 Conclusion

This Sales Analysis dashboard demonstrates how raw sales data can be transformed into meaningful business insights using Power BI. By leveraging interactive visuals and key performance metrics, the dashboard enables stakeholders to monitor performance, identify opportunities, and support data-driven decision-making.

The project showcases practical skills in data preparation, DAX calculations, and dashboard design using Power BI Desktop.

📥 How to Use This Project

Download the .pbix file from this repository or the provided Power BI Desktop link.

Open the file using Power BI Desktop.

Use slicers and visuals to explore different aspects of the sales data.

👤 Author

Amal Samad
Data Analyst | Power BI | SQL | Python
