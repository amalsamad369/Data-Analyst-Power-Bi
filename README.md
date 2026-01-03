# Sales Analysis Dashboard

## Problem Statement

The purpose of this project is to analyze sales performance using historical sales data and present the findings through an interactive Power BI dashboard. The dashboard is designed to help business stakeholders understand overall sales trends, profitability, customer behavior, and regional performance.

By analyzing key sales indicators such as total sales, profit, quantity sold, and order volume, this dashboard enables decision-makers to identify high-performing products, underperforming regions, and seasonal trends. The insights derived from this analysis can support strategic planning, inventory management, and revenue optimization.



### Steps followed 

- Step 1 :The sales dataset was loaded into Power BI Desktop from a CSV file.
- Step 2 :The Power Query Editor was opened, and under the View tab, the options Column Distribution, Column Quality, and Column Profile were enabled to analyze data quality.
- Step 3 : Since column profiling is enabled only for the first 1000 rows by default, “Column profiling based on entire dataset” was selected to ensure complete data analysis
- Step 4 : Data profiling showed that most columns were clean, with only minimal missing values in some numeric fields.
- Step 5 : The missing values were less than 1% of the dataset. Therefore, blank values were ignored during average and ratio calculations to maintain accuracy.
- Step 6 : In the Report View, a suitable theme was selected from the View tab to ensure a consistent and professional dashboard appearance.
- Step 7 : Multiple visuals were added to represent key metrics such as sales, profit, and order count.
- Step 8 : Slicers were added to enable interactive filtering of the data based on dimensions like Region, Category, Sub-Category, and Date.
- Step 9 : Card visuals were used to display important KPIs such as:
    
    - Total Sales

   - Total Profit

   -  Total Orders
- Step 10 : A Bar Chart was used to analyze Sales by Category, allowing comparison across product categories. 
- Step 11 : A Line Chart was created to visualize the Monthly Sales Trend, helping identify patterns and seasonality.
- Step 12 : A Profit Analysis visual was included to understand profit distribution across different categories and regions.
- Step 13 : Text boxes were added using the Insert tab to display the dashboard title and a brief description. 
- Step 14 : Design elements such as shapes and the company logo were added to enhance the visual appeal of the report.
for creating new column following DAX expression was written;
       
       Date Table 1 = CALENDARAUTO()

        
Snap of new calculated column ,

<img src="https://github.com/user-attachments/assets/944fe74a-b0f3-4f6e-b5c5-83a07a1ca42a" width="400"/>


        
- Step 15 :A measure Quantity Sold was created to calculate total units sold by activating an inactive date relationship.
        
      Quantity Sold = CALCULATE =( SUM('Fact Table'[Units Sold]),ALL('Date Table 1'),USERELATIONSHIP('Date Table 2'[Date], 'Fact Table'[Date (dd/mm/yyyy)])
               
 - Step 16 :A measure Sum of Net Sales was created to calculate total net sales using an alternate date relationship.
 
 
         Sum of Net Sales = CALCULATE( SUM('Fact Tabl[Net Sales]),ALL('Date Table 1'),USERELATIONSHIP('Date Table 2'[Date], 'Fact Table'[Date (dd/mm/yyyy)]))
 
 - Step 17 : A measure Total Profit was created to calculate overall profit by enabling an inactive date relationship.
 
 Following DAX expression was written to find total profit,
 
         Total profit = CALCULATE(SUM('Fact Table'[Profit]), ALL('Date Table 1'),
    USERELATIONSHIP('Date Table 2'[Date], 'Fact Table'[Date (dd/mm/yyyy)]))
    
 A card visual was used to represent this total profit.
 
 
 <img width="359" height="114" alt="Image" src="https://github.com/user-attachments/assets/2e338d75-db3a-4809-b40d-e8d8231e8905" />

 # Report Snapshot (Power BI DESKTOP)
<img width="1919" height="1022" alt="Image" src="https://github.com/user-attachments/assets/a3d7e9ae-eb76-4db9-9996-4ad9e208592a" />)

# Insights

A single-page interactive Sales Analytics report was developed using Power BI Desktop. The dashboard provides insights into sales performance, revenue, profitability, and customer behavior.

Following inferences can be drawn from the dashboard;

### [1] Overall Sales Performance
Total Quantity Sold: Calculated across all transactions using an alternate date relationship.

Total Net Sales: Represents overall revenue generated from sales.

Total Profit: Indicates profitability after accounting for costs.

 


           Sales and profit figures vary significantly across time periods and are influenced by date-based filters applied through slicers
           
### [2] Sales Trend Analysis

Sales show noticeable variation across different months and years.

Certain periods contribute disproportionately higher sales and profit.

    Peak sales periods can be identified, helping businesses plan inventory and marketing strategies effectively.
 
  
  ### [3] Product Performance 
  
      High-volume, low-margin products should be reviewed for pricing or cost optimization

A small set of products contributes the majority of total sales.
Some products generate high sales volume but comparatively lower profit margins..

 ### [4] Profitability Analysis
 
 Profit does not always increase proportionally with sales.

Some regions or product categories contribute negatively to profit.
 
         Loss-making segments require corrective actions such as cost reduction or pricing revision.
 
 ### [5] Impact of Filters
 
 All metrics dynamically change with slicers such as date, product category, region, and customer segment.
 
         Interactive filtering enables detailed drill-down analysis for informed decision-making.
         

