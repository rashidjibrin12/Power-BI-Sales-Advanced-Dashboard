# Power BI Sales Advanced Dashboard

This project is a sales dashboard built in Power BI using a realistic B2B industrial sales dataset. It combines transaction-level sales data with product, customer, region, and sales rep information to give a clearer picture of performance across revenue, profit, targets, and discounts.

The goal was to build something that feels close to how a real sales team would look at business performance—tracking what is selling, where it is selling, who is driving the results, and where the biggest opportunities are.

The dashboard helps answer practical questions like:
- Which products and categories are generating the most revenue and profit?
- Which regions and sales reps are outperforming the portfolio average?
- Are actual sales tracking above or below target and forecast levels?
- How do discounts, order size, and product mix affect margin?
- Where are the biggest opportunities for growth, margin improvement, or sales coverage?

The data model follows a star schema, with a central fact table at the center of the analysis and supporting dimension tables providing context around each transaction.

## Data Sources
- FactSales.csv — Transactional sales data including order date, ship date, product, customer, region, sales rep, quantity, unit price, discount, revenue, profit, target, and forecast
- DimProducts.csv — Product details, including category and subcategory
- DimCustomers.csv — Customer profiles and B2B segment classification
- DimRegions.csv — Geographic and country mapping for sales territories
- DimSalesReps.csv — Sales rep assignments by territory

## What the data tells us
A few patterns stand out from the dataset:

### 1) This is a B2B, project-driven sales environment
The data is built around business accounts, territories, and sales reps rather than a retail-style customer mix. Each order connects to a product, customer, and geography, which makes the analysis much more relevant for operational sales planning and territory management.

### 2) Revenue is concentrated in a smaller set of high-value products
The biggest revenue spikes come from premium industrial items with higher unit prices and larger order volumes. In other words, a relatively small number of products are responsible for a meaningful share of total sales value.

### 3) Profitability is strongest when pricing and order mix work in the company’s favor
The data suggests that higher-value orders in premium product groups often produce the strongest absolute profit. At the same time, lower-priced items can be harder to grow profitably unless the economics are favorable.

### 4) Discounts have a noticeable impact on margins
Discounting is clearly part of the operating model, and it can meaningfully reduce overall profitability. Some higher-revenue deals still produce weaker margins when discount rates are too aggressive.

### 5) Regional performance is uneven, but still informative
Performance is not evenly distributed across countries and territories. Some territories are stronger because of larger order values or a more favorable mix of products, while others are more constrained by lower volume or weaker pricing power.

### 6) Targets and forecasts are useful, but large orders create spikes
The dataset includes both target and forecast values, which makes it useful for comparing actual performance against expectations. The results generally track well, but large individual orders can create noticeable jumps that are important to understand when evaluating performance.

### 7) The sales pattern feels realistic and operationally grounded
The data includes everything from smaller transactions to multi-thousand-dollar orders, which gives the model a believable spread of business activity. That makes it a strong example of a practical sales dataset rather than something overly simplified or synthetic.

## Tools Used
- Microsoft Power BI Desktop
- Power Query for data import and transformation
- DAX for KPI and performance calculations
- CSV-based source files for sales and dimension tables
- GitHub for version control and project documentation

## Screenshot
<img width="1696" height="951" alt="Power BI executive sales dashboard screenshot" src="https://github.com/user-attachments/assets/7b7e57b5-228c-4b51-a19c-9053ea156273" />

## Executive Summary
This project is a practical example of how a sales dashboard can turn raw data into something useful for decision-making. The dataset reflects a realistic industrial sales environment where revenue, margin, territory performance, and discounting all matter together. The dashboard helps make those trade-offs easier to see and act on.
