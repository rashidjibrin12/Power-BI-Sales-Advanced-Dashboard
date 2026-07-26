# Power BI Sales Advanced Dashboard

This repository contains a Power BI report and the dataset files used to build the Sales Advanced dashboard.

## Power BI Desktop file (PBIX)

- File: [Power BI Advanced.pbix](./Power%20BI%20Advanced.pbix)
- Size: 328,678 bytes (included in repository)

Description

This PBIX file contains the interactive Sales Advanced dashboard built with Power BI Desktop. It uses the CSV datasets included in this repository as its data source. The report provides interactive visualizations for sales metrics and supports filtering, drill-downs, and cross-highlighting.

Datasets included in this repository (used by the PBIX file)

- `FactSales.csv` — transactional sales data
- `DimCustomers.csv` — customer dimension
- `DimProducts.csv` — product dimension
- `DimRegions.csv` — region dimension
- `DimSalesReps.csv` — sales representative dimension

How to open and explore

1. Download the `Power BI Advanced.pbix` file from this repository.
2. Open it using Power BI Desktop (download latest stable release from Microsoft if you don't have it).
3. If the report cannot find the CSV files, point the PBIX file to the CSV files in this repository (File -> Options and settings -> Data source settings -> Change Source) or copy the CSV files locally and update the file paths.
4. Refresh the report (Home -> Refresh) to load the latest data from the CSV files.

Notes for contributors

- If you update the PBIX file, please include the updated .pbix in the repository and note in the commit message which pages or visuals were changed.
- To change or extend the dataset, modify the CSV files or reconnect the PBIX to an external data source and include instructions in the README describing the new connection details.

License

See the repository root for license information (if provided).
