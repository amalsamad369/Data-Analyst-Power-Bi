# UPI Transactions Analysis Dashboard

## Problem Statement

The purpose of this project is to analyze UPI transaction data using historical transaction records and present the insights through an interactive Power BI dashboard. The dashboard is designed to help stakeholders understand transaction behavior, balance trends, user demographics, and city-wise payment patterns.

By analyzing key UPI indicators such as transaction amount, remaining balance, transaction type, payment method, and customer attributes, this dashboard enables better understanding of digital payment usage patterns. The insights derived from this analysis can support decision-making related to financial monitoring, user behavior analysis, and operational planning.



### Steps followed 

#### Step 1:
The UPI transactions dataset was loaded into Power BI Desktop from an Excel file.

#### Step 2:
The Power Query Editor was opened, and under the View tab, Column Distribution, Column Quality, and Column Profile options were enabled to assess data quality.

####  Step 3:
Since column profiling is enabled only for the first 1000 rows by default, “Column profiling based on entire dataset” was selected to ensure complete data analysis.

#### Step 4:
Data profiling showed that most columns were clean, with minimal missing values in numeric fields such as transaction amount and remaining balance.

#### Step 5:
As missing values were negligible, blank records were ignored during aggregation and calculations to maintain analytical accuracy.

#### Step 6:
In the Report View, a suitable theme was selected from the View tab to maintain a consistent and professional dashboard layout.

#### Step 7:
Multiple visuals were added to represent key UPI metrics such as transaction amounts and remaining balances.

#### Step 8:
 -Slicers were added to enable interactive filtering based on:

- City

- Bank Name (Sent & Received)

- Merchant Name

- Payment Method

- Device Type

- Gender

- Age Group

- Purpose

- Transaction Type



#### Step 9:
A Matrix Visual was created to display Month-wise and City-wise Transaction Amount and Remaining Balance, allowing detailed comparative analysis.

#### Step 10:
Line Charts were created to analyze:

Monthly Transaction Amount trends

Monthly Remaining Balance trends

#### Step 11:
Column Charts were added to compare:

Transaction Amount by Month

Remaining Balance by Month

#### Step 12:
Conditional Formatting was applied in matrix visuals to highlight higher and lower transaction values for quick interpretation.

#### Step 13:
Bookmarks were created to toggle between:

- Transaction Amount visuals

- Remaining Balance visuals

#### Step 14:
Text boxes were added to display dashboard titles and descriptions, and layout elements were aligned for better readability.
 
 
 #### Step 15:
Measures were created using DAX to calculate total transaction amounts and remaining balances dynamically based on slicer selections.

#### Step 17:
The report was optimized and prepared for publishing, with slicer synchronization applied across pages for a seamless user experience.

# Report Snapshot (Power BI Desktop)

### Page 1 – Monthly Balance Analysis
<img width="1919" height="1002" alt="Image" src="https://github.com/user-attachments/assets/27246137-d40d-40ed-a319-61cf4249992e" />

### Page 2 – City-wise Matrix with Conditional Formatting
<img width="1907" height="993" alt="Image" src="https://github.com/user-attachments/assets/debfe02b-678a-4a28-8732-5a0cbb7e6d18" />



# Insights

Insights

A multi-page interactive UPI Transactions Analytics dashboard was developed using Power BI Desktop. The dashboard provides insights into digital payment behavior, transaction volume, and balance trends across different cities and user demographics.

Following inferences can be drawn from the dashboard:

### [1] Overall UPI Transaction Performance

Transaction amounts vary significantly across months and cities.

Remaining balance trends indicate periodic spikes and drops linked to transaction activity.

Transaction behavior is strongly influenced by filters such as city, payment method, and transaction type.

###  [2] Monthly Transaction Trend Analysis

Certain months record noticeably higher transaction volumes.

Seasonal patterns can be observed in both transaction amounts and balances.

Peak transaction periods can help identify high-usage phases in digital payments.

###  [3] City-wise Analysis

Major cities contribute a higher share of UPI transactions.

Some cities show higher transaction frequency but lower remaining balances.

City-wise comparison helps identify regional usage intensity.

###  [4] User & Payment Behavior Analysis

Transaction behavior differs across age groups and gender.

Device type and payment method significantly influence transaction patterns.

Understanding user demographics enables targeted financial analysis and service optimization.

