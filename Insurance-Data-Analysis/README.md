# Insurance Analytics Dashboard


## Problem Statement

The objective of this project is to analyze insurance policy and claims data sourced from a Microsoft SQL Server database and present actionable insights through an interactive Power BI dashboard. The dashboard enables stakeholders to understand premium distribution, claim trends, customer behavior, and policy performance.

By leveraging drill-through analysis, row-level security, scheduled refresh, and sentiment analysis, the solution supports secure, real-time, and role-based decision-making for insurance operations.



### Steps followed 

- Step 1: Insurance data was connected and loaded into Power BI Desktop directly from Microsoft SQL Server.

- Step 2: Relevant tables were selected, relationships were validated, and data types were verified.

- Step 3: Power Query Editor was used to assess data quality by enabling Column Distribution, Column Quality, and Column Profile.

- Step 4: Column profiling was applied to the entire dataset to ensure complete data validation.

- Step 5: Data cleaning was performed to handle missing values, duplicates, and inconsistent formats.

- Step 6: Minor missing values were ignored during calculations to maintain analytical accuracy.

- Step 7: A professional and consistent report theme was applied.

- Step 8: Core visuals were created to represent premium amount, claim amount, policy count, and claim ratio.

-  Step 9: Slicers were added to enable interactive filtering by Policy Type, Region, Customer Segment, and Date.

- Step 10: Card visuals were used to display key KPIs:

-Total Policies

-Total Premium Amount

-Total Claim Amount

Claim Ratio

- Step 11:Drill-through filters were implemented to enable detailed analysis of insurance claims and policies by region, customer, and policy type. This feature allows users to right-click on a visual and navigate to a detailed report page for deeper insights.
### Drill-through Page Snapshot:
<img width="1881" height="991" alt="Image" src="https://github.com/user-attachments/assets/864c398b-17ee-4e42-ba4d-e4d970513a5d" />


- Step 12: A Line Chart was created to visualize claim and premium trends over time.

- Step 13: Sentiment analysis was performed in Power Query on customer feedback data to classify sentiments into Positive, Neutral, and Negative categories, enabling qualitative assessment of customer satisfaction.

### Power Query – Sentiment Analysis Snapshot:
<img width="1243" height="715" alt="Image" src="https://github.com/user-attachments/assets/b98f8096-138d-42fe-95ea-5aaef9e130ea" />



- Step 14: Text boxes, shapes, and icons were added to enhance report clarity and visual appeal.

- Step 15: Row-Level Security (RLS) was implemented to restrict data access based on user roles and regions.

- Step 16: The report was published to Power BI Service, and scheduled data refresh was configured to ensure up-to-date reporting.

 # Report Snapshot (Power BI DESKTOP)
<img width="1919" height="1017" alt="Image" src="https://github.com/user-attachments/assets/a4758331-4235-4f26-9f69-f125e8a7f221" />

# Insights

A single-page interactive Insurance Analytics dashboard was developed using Power BI with SQL Server as the data source.

### [1] Overall Insurance Performance

Total Premium and Total Claims provide a clear view of revenue and risk exposure.
Claim Ratio highlights policy profitability and underwriting efficiency.

### [2] Claim & Premium Trends

Claims and premiums vary across time periods, revealing seasonal patterns and high-risk intervals.

### [3] Customer & Policy Analysis

Drill-through analysis enables deep inspection of individual policies and customer-level claim behavior.
Sentiment analysis highlights customer satisfaction levels and potential service issues.

### [4] Security & Automation

Row-Level Security ensures data confidentiality for regional and role-based users.
Scheduled refresh guarantees near real-time insights without manual intervention.

### [5] Impact of Filters

All KPIs and visuals dynamically update using slicers and drill-through filters, enabling detailed and secure decision-making.
