# Customer_Segmentation-using-RFM-Analysis-Task-15
Customer Segmentation using RFM (Recency, Frequency, Monetary) analysis on retail transaction data. This project cleans and processes customer purchase data using Python, calculates RFM scores, segments customers into meaningful groups, and provides business action strategies for each segment to support targeted marketing and customer retention.

# Overview
This project performs Customer Segmentation using the RFM (Recency, Frequency, Monetary) model. The goal is to identify different types of customers based on their purchasing behavior and provide actionable business insights.

# Objective
 - Analyze customer purchase behavior
 - Calculate RFM metrics
 - Segment customers into meaningful groups
 - Suggest marketing actions for each segment

# Dataset
- The dataset contains e-commerce transaction data with the following columns:
    - InvoiceNo
    - StockCode
    - Description
    - Quantity
    - InvoiceDate
    - UnitPrice
    - CustomerID
    - Country

- For RFM analysis, the following columns were used:
    - CustomerID
    - InvoiceNo
    - InvoiceDate
    - Quantity
    - UnitPrice

# Tools & Technologies
 - Python
 - Pandas, NumPy, Matplotlib
 - Jupyter Notebook

# Data Cleaning Steps
 - Removed rows with missing CustomerID
 - Removed cancelled invoices
 - Removed negative or zero quantities
 - Converted InvoiceDate to datetime format
 - Created a new column:
     - TotalAmount = Quantity × UnitPrice

# RFM Analysis Steps
 1. Calculated Recency:
       - Days since last purchase
 2. Calculated Frequency:
       - Number of unique invoices per customer
 3. Calculated Monetary:
       - Total amount spent by customer
 4. Assigned RFM scores using quantiles.
 5. Combined scores into a single RFM score.
 6. Segmented customers into groups:
       - Champions         (Recent, frequent, and high-spending customers)
       - Loyal Customers   (Regular customers with strong purchase history)
       - At Risk           (Previously active but not recent buyers)
       - Regular Customers (Average customers with moderate activity)
   
# Key Insights
 - Identified top-value customers (Champions).
 - Detected customers at risk of churn.
 - Observed distribution of customers across segments.

# Project Files
 - task15_rfm.ipynb → RFM analysis notebook
 - rfm_segments.csv → Final segmented customer data
 - segment_actions.txt → Marketing actions for each segment
 - README.md → Project documentation

# Learning Outcomes
 - Understanding RFM analysis
 - Customer behavior analysis
 - Data cleaning and preprocessing
 - Customer segmentation techniques
 - Business-driven data insights

# Conclusion
 This project demonstrates how businesses can use RFM analysis to understand customer behavior and design targeted marketing strategies for different customer segments.
