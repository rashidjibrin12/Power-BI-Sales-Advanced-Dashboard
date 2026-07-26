# Power BI Sales Advanced Dashboard

This repository contains a Power BI report and the dataset files used to build the Sales Advanced dashboard.

## About this project

This project demonstrates how to build an interactive sales analytics dashboard using Power BI Desktop. It includes an example sales dataset and a pre-built PBIX report that showcases common business intelligence features such as KPI cards, trend charts, geographic maps, drill-throughs, slicers, and cross-highlighting. The data model follows a simple star schema (one fact table with several dimension tables) so it's easy to explore, extend, and adapt to real-world datasets.

Target audience: data analysts, business users, and developers who want a starting template for sales reporting and visualization in Power BI.

## Files included

- `Power BI Advanced.pbix` — Power BI Desktop report file containing the interactive dashboard (path: `Power BI Advanced.pbix`).
- `FactSales.csv` — transactional sales data used as the fact table (path: `FactSales.csv`).
- `DimCustomers.csv` — customer dimension (path: `DimCustomers.csv`).
- `DimProducts.csv` — product dimension (path: `DimProducts.csv`).
- `DimRegions.csv` — region dimension (path: `DimRegions.csv`).
- `DimSalesReps.csv` — sales representative dimension (path: `DimSalesReps.csv`).
- `README.md` — this file with usage instructions and documentation.

(If you add other files later, list them here with a short description.)

## Key insights and visuals

The report is designed to surface common sales and business insights. Example insights you can explore in the dashboard:

- Total sales, orders, and average order value (KPI cards).
- Sales trend over time (daily/monthly/quarterly) and seasonality patterns.
- Top-performing products and product categories by revenue and quantity sold.
- Regional sales performance and geographic distribution of revenue.
- Customer segmentation by revenue and order frequency (top customers vs long-tail).
- Sales representative performance and leaderboard.
- Product or region drill-through pages that show transaction-level details.
- Filters and slicers for time period, product category, region, and sales rep to answer ad-hoc questions.

These visuals help stakeholders quickly identify growth opportunities, underperforming areas, and high-value customers.

## Steps to open, explore, and refresh the report

1. Download the `Power BI Advanced.pbix` file from this repository.
2. Install Power BI Desktop (get the latest stable version from Microsoft if you don't already have it).
3. Open `Power BI Advanced.pbix` in Power BI Desktop.
4. If visuals show errors because the PBIX cannot find the CSV files, update the data source:
   - Go to File -> Options and settings -> Data source settings -> Change Source.
   - Point the file paths to the local copies of the CSV files or set the folder path where the CSV files reside.
   - Alternatively, copy the CSV files into the same relative location the PBIX expects.
5. Refresh the dataset (Home -> Refresh) so Power BI re-reads the CSV files and loads the latest data.
6. Interact with the report:
   - Use slicers to filter by date range, region, product, or sales rep.
   - Click visuals to cross-filter and drill down/up where supported.
   - Use drill-through pages for transaction-level analysis.
7. Exporting and sharing:
   - Export a report page as PDF (File -> Export -> PDF) or export data from a visual (right-click a visual -> Export data).
   - If you have Power BI Service, publish the PBIX to your workspace to share dashboards and set up scheduled refreshes (requires data to be accessible from the service or via a gateway).

Tips

- If the report hangs during refresh, try disabling unnecessary visuals or increasing Power BI's memory by running fewer other applications.
- Use parameters for file paths when you want contributors to point the PBIX to local files without editing queries.
- To publish to Power BI Service and schedule refreshes, place the CSV files in a cloud storage (OneDrive/SharePoint) or configure an on-premises gateway.

## How the data model is structured

The PBIX uses a star schema:

- Fact table: `FactSales` (transactions, measures like Sales Amount, Quantity, Cost)
- Dimension tables: `DimProducts`, `DimCustomers`, `DimRegions`, `DimSalesReps`

Relationships are one-to-many from each dimension table to the fact table on their respective keys.

## Contributions

- If you update the PBIX, please include the updated `.pbix` file and describe the changes in the commit message (e.g., "Updated Product detail page, added YOY measure").
- For changes to the dataset, update the CSV files and include a note describing the data source and any transformation logic used.

## License

See the repository root for license information (if provided).
