# Sales Analysis Dashboard

### Dashboard Link : https://app.powerbi.com/groups/me/reports/384d017e-e935-44dc-9e7d-1626c1a36de1/ReportSection

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


        
- Step 15 : New measure was created to find total count of customers.

Following DAX expression was written for the same,
        
        Count of Customers = COUNT(airline_passenger_satisfaction[ID])
        
A card visual was used to represent count of customers.

![Snap_Count](https://user-images.githubusercontent.com/102996550/174090154-424dc1a4-3ff7-41f8-9617-17a2fb205825.jpg)

        
 - Step 16 : New measure was created to find  % of customers,
 
 Following DAX expression was written to find % of customers,
 
         % Customers = (DIVIDE(airline_passenger_satisfaction[Count of Customers], 129880)*100)
 
 A card visual was used to represent this perecntage.
 
 Snap of % of customers who preferred business class
 
 ![Snap_Percentage](https://user-images.githubusercontent.com/102996550/174090653-da02feb4-4775-4a95-affb-a211ca985d07.jpg)

 
 - Step 17 : New measure was created to calculate total distance travelled by flights & a card visual was used to represent total distance.
 
 Following DAX expression was written to find total distance,
 
         Total Distance Travelled = SUM(airline_passenger_satisfaction[Flight Distance])
    
 A card visual was used to represent this total distance.
 
 
 ![Snap_3](https://user-images.githubusercontent.com/102996550/174091618-bf770d6c-34c6-44d4-9f5e-49583a6d5f68.jpg)
 
 - Step 18 : The report was then published to Power BI Service.
 
 
![Publish_Message](https://user-images.githubusercontent.com/102996550/174094520-3a845196-97e6-4d44-8760-34a64abc3e77.jpg)

# Snapshot of Dashboard (Power BI Service)

![dashboard_snapo](https://user-images.githubusercontent.com/102996550/174096257-11f1aae5-203d-44fc-bfca-25d37faf3237.jpg)

 
 # Report Snapshot (Power BI DESKTOP)

 
![Dashboard_upload](https://user-images.githubusercontent.com/102996550/174074051-4f08287a-0568-4fdf-8ac9-6762e0d8fa94.jpg)

# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] Total Number of Customers = 129880

   Number of satisfied Customers (Male) = 28159 (21.68 %)

   Number of satisfied Customers (Female) = 28269 (21.76 %)

   Number of neutral/unsatisfied customers (Male) = 35822 (27.58 %)

   Number of neutral/unsatisfied customers (Female) = 37630 (28.97 %)


           thus, higher number of customers are neutral/unsatisfied.
           
### [2] Average Ratings

    a) Baggage Handling - 3.63/5
    b) Check-in Service - 3.31/5
    c) Cleanliness - 3.29/5
    d) Ease of online booking - 2.88/5
    e) Food & Drink - 3.21/5
    f) In-flight Entertainment - 3.36/5
    g) In-flight service - 3.64/5
    h) In-flight Wifi service - 2.81/5
    i) Leg room service - 3.37/5
    j) On-board service - 3.38/5
    k) Online boarding - 3.33/5
    l) Seat comfort - 3.44/5
    m) Departure & arrival convenience - 3.22/5
  
  while calculating average rating, null values have been ignored as they were not relevant for some customers. 
  
  These ratings will change if different visual filters will be applied.  
  
  ### [3] Average Delay 
  
      a) Average delay in arrival(minutes) - 15.09
      b) Average delay in departure(minutes) - 14.71
Average delay will change if different visual filters will be applied.

 ### [4] Some other insights
 
 ### Class
 
 1.1) 47.87 % customers travelled by Business class.
 
 1.2) 44.89 % customers travelled by Economy class.
 
 1.3) 7.25 % customers travelled by Economy plus class.
 
         thus, maximum customers travelled by Business class.
 
 ### Age Group
 
 2.1)  21.69 % customers belong to '0-25' age group.
 
 2.2)  52.44 % customers belong to '25-50' age group.
 
 2.3)  25.57 % customers belong to '50-75' age group.
 
 2.4)  0.31 % customers belong to '75-100' age group.
 
         thus, maximum customers belong to '25-50' age group.
         
### Customer Type

3.1) 18.31 % customers have customer type 'First time'.

3.2) 81.69 % customers have customer type 'returning'.
       
       thus, more customers have customer type 'returning'.

### Type of travel

4.1) 69.06 % customers have travel type 'Business'.

4.2) 30.94 % customers have travel type 'Personal'.

        thus, more customers have travel type 'Business'.



Use slicers and visuals to explore different aspects of the sales data.

👤 Author

Amal Samad
Data Analyst | Power BI | SQL | Python
