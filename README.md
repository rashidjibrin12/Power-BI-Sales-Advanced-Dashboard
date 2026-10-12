# Power BI Sales Advanced Dashboard

## Project Overview
This repository contains a Power BI sales analytics project built around a realistic B2B industrial sales dataset. The model combines transaction-level sales data with product, customer, region, and sales representative dimensions to support executive review of performance, profitability, and planning.

The dashboard is designed to answer practical business questions such as:
- Which products and categories are producing the most revenue and profit?
- Which regions and sales reps are outperforming the portfolio average?
- Are actual sales tracking above or below target and forecast levels?
- How do discounts, order size, and product mix affect margin?
- Where are the biggest opportunities for growth, margin improvement, or sales coverage?

The data model follows a star schema with a central fact table (FactSales.csv) and supporting dimensions (DimProducts.csv, DimCustomers.csv, DimRegions.csv, and DimSalesReps.csv). This structure is consistent with typical business intelligence reporting used in manufacturing, industrial distribution, and sales operations.

## Data Sources
- FactSales.csv — Transactional sales records including order date, ship date, product, customer, region, sales rep, quantity, unit price, discount, revenue, profit, target, and forecast
- DimProducts.csv — Product data with category and subcategory
- DimCustomers.csv — Customer data and B2B segment classification
- DimRegions.csv — Geographic and country mapping for sales territories
- DimSalesReps.csv — Sales rep assignments by territory

## Key Findings
The dashboard highlights several practical business insights:

### 1) The business is B2B and project-driven rather than retail
The sales data is built around a limited number of business accounts, territories, and representatives, with each order tied to products, customers, and geography. The presence of sales reps, region mapping, and industrial product categories suggests a manufacturing or distribution context rather than consumer retail.

### 2) Revenue is driven by a small number of high-value products
The most meaningful revenue spikes come from premium industrial items with high unit prices and larger order quantities. Products in the higher-value segment generate the largest order values. These products are the main contributors to overall revenue, even though they may not be the highest-volume items.

### 3) Profitability is strongest where pricing and order mix are favorable
The data shows a clear relationship between order size, price point, and margin performance. Larger orders in premium categories often produce the strongest absolute profit, while lower-priced products can still generate volume but contribute less to total profit. This makes the dashboard useful for evaluating not just revenue growth, but margin quality.

### 4) Discounting materially affects profitability
Discounts appear in the dataset as an operational lever, and they can materially compress broader profit performance. Some higher-revenue transactions still produce lower margins if discount rates are elevated, which is a realistic observation in industrial sales where negotiated pricing and customer-specific terms are common.

### 5) Regional performance is uneven but strategic
The data includes multiple countries and territories, and performance is not evenly distributed. Some territories show stronger revenue concentration due to larger order values or more repeated high-transaction activity, while others are more moderate. This supports the idea that the dashboard is useful for territory-level sales planning and resourcing decisions.

### 6) Target and forecast track sales activity, but large orders create spikes
The presence of Target and Forecast columns is important: the dashboard is designed to compare actual performance against expected performance. The dataset shows that actual sales often align well with expectations, but notable deviations occur when large, high-priority orders arrive. These deviations make it valuable to monitor both trend and exception performance, not just the average.

### 7) The sales pattern is operationally realistic
The data includes a broad range of order values—from smaller orders to large multi-thousand-dollar transactions—with a realistic mix of low-value and premium-value orders. This is a strong sign that the dataset was designed to mimic real B2B sales behavior rather than a simplified or artificially flat scenario.

## Tools Used
- Microsoft Power BI Desktop
- Power Query for data import and transformation
- DAX for KPI and performance calculation
- CSV-based source files for sales and dimension tables
- GitHub for version control and project documentation

## Screenshot
<img width="1696" height="951" alt="Power BI executive sales dashboard screenshot" src="https://github.com/user-attachments/assets/7b7e57b5-228c-4b51-a19c-9053ea156273" />

## Executive Summary
This project demonstrates a realistic and analytically useful Power BI implementation for industrial sales performance management. The dataset shows a sales environment where revenue generation is concentrated in a handful of premium products and territories, while profitability depends on pricing discipline, order size, and discount management. The dashboard is well suited for answering enterprise questions around performance trends, sales rep effectiveness, regional contribution, and target-versus-actual sales outcomes.














































