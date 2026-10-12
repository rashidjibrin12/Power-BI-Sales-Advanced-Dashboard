# Power BI Executive Dashboard

## Project Overview
This project is a sales performance dashboard built in Power BI to analyze transactional sales data across products, customers, regions, and sales representatives. The dashboard is designed to help stakeholders quickly understand business performance, compare actual results to targets and forecasts, and identify growth opportunities or decline areas.

The data model is structured as a star schema with a central fact table for transactions and supporting dimension tables for product, customer, region, and sales rep details. The report is intended to function as a business intelligence starter project that demonstrates practical dashboard design and analytic storytelling in Power BI.

## Business Question
The dashboard answers a few core business questions:

- Which products, categories, and regions are generating the most revenue and profit?
- How do current sales compare against target and forecast performance?
- Which sales representatives are performing best by territory and contribution?
- Are there customer segments or regions where sales performance is underperforming?
- How can the business use sales trend data to improve planning and decision-making?

## Skills Demonstrated
This project demonstrates a range of business intelligence and analytics skills, including:

- Power BI dashboard design and report development
- Data modeling using star schema relationships
- Data transformation and preparation from CSV sources
- DAX measure creation for KPIs, profit, forecasting, and variance analysis
- Sales trend analysis and performance monitoring
- Business storytelling through executive-friendly visuals and KPI cards
- Customer, product, and regional segmentation analysis
- Dashboard interactivity using slicers, drill-down, and filtering

## Tools Used
- Microsoft Power BI Desktop
- Power Query for data import and shaping
- DAX for calculated measures and custom logic
- CSV data files as source datasets
- GitHub for repository management and documentation

## Datasets
The project uses a set of structured sales and dimension tables:

- FactSales.csv — transaction-level sales fact table containing order dates, revenue, profit, quantity, discounts, target, and forecast values
- DimProducts.csv — product master data including product names, categories, and subcategories
- DimCustomers.csv — customer names and customer segment information
- DimRegions.csv — region and country mapping across sales territories
- DimSalesReps.csv — sales representative assignments by region

This dataset is representative of a B2B industrial sales environment with transactional records spanning multiple dates and business units.

## Key Findings
The dashboard is structured to reveal several important business insights:

- Revenue and profit are driven largely by high-value product lines and premium industrial categories.
- Product category and regional performance vary significantly, which suggests opportunities for targeted sales planning and resource allocation.
- Sales rep performance can be compared across territories to identify top performers and coaching opportunities.
- Target-versus-actual performance analysis helps highlight where revenue is exceeding or falling short of expectations.
- Discounting, product mix, and territory concentration are likely key drivers of margin and profitability.
- The dataset supports both operational reporting and strategic analysis, making it suitable for business review and weekly sales tracking.

<img width="1696" height="951" alt="{BE227752-3EBB-439C-B9A2-9557DDB244ED}" src="https://github.com/user-attachments/assets/7b7e57b5-228c-4b51-a19c-9053ea156273" />


## Final Summary
By combining product, customer, region, and sales representative views, the project demonstrates practical business intelligence capabilities that are highly relevant for data analytics, sales operations, and performance reporting roles.

