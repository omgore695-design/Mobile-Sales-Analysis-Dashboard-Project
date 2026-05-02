# Mobile-Sales-Analysis-Dashboard-Project
Developed a comprehensive Business Intelligence (BI) dashboard to track and analyze mobile phone sales performance across multiple regions. The project provides stakeholders with actionable insights into revenue trends, customer demographics, and product-level performance to optimize inventory and marketing strategies.
1. Project Summary
This repository contains a comprehensive Mobile Sales Analysis Dashboard. The
project transforms raw sales data into dynamic visualizations, enabling retail
managers to track key performance indicators (KPIs) across different regions,
mobile brands, and customer demographics.
Power BI Desktop DAX Query Language Power Query Data Modeling

2. Objectives
Sales Tracking: Monitor daily and monthly sales performance.
Product Insight: Identify top-performing mobile brands (Apple, Samsung, etc.)
and specifications (RAM, Storage).
Customer Behavior: Segment sales by gender and age group for targeted
marketing.
Inventory Planning: Analyze sales volume by model to optimize stock levels.

3. Data Structure
The dashboard is built on a relational data model (Star Schema):
Sales_Fact : Transactional data including Price, Quantity, and Revenue.
Product_Dim : Handset details, brand names, and storage variants.
Calendar_Dim : Standardized dates for Time Intelligence functions.
Customer_Dim : Demographics and location details.

4. Key Performance Indicators (KPIs)
The following DAX measures are implemented in the dashboard:
Total Sales = SUM(Sales[Revenue])
Avg Order Value = DIVIDE([Total Sales], COUNT(Sales[TransactionID]))
Top Brand = TOPN(1, VALUES(Product[Brand]), [Total Sales])

5. Dashboard View
Summary View: High-level overview of revenue, transactions, and profit.
Regional Analysis: Map visual showcasing performance by city.
Product Breakdown: Donut charts for Brand share and Model popularity.
Filters: Slicers for Date Range, Region, and Mobile Brand.
6. How to Use
Download the Mobile_Sales_Project.pbix file.
Ensure the data source (Excel/CSV) is located in the same directory.
Open the file in Power BI Desktop.
Select Transform Data to update file paths if necessary.
Use the interactive slicers on the right to explore specific timeframes or
regions.

