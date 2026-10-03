# BrewMetrics Coffee Sales Dashboard

## Project Overview

BrewMetrics is a Power BI dashboard for exploring coffee sales across cities, products, and dates. The project uses a CSV sales dataset and a Power BI semantic model, with GitHub for version control and GitHub Copilot to assist with DAX development.

## Data Model

The semantic model uses a sales fact table with three dimensions:

- **Fact_Sales** — sales records, including sale ID, date, city, store format, category, item, quantity, unit price, sales amount, and a generated product key.
- **Dim_Date** — distinct dates from the sales data.
- **Dim_City** — distinct cities from the sales data.
- **Dim_Product** — distinct category, store format, and item combinations, with a generated product key.

The fact table is related to the dimensions through date, city, and product keys. The product key is formed from category, item, and store format. A hidden Power BI local date table supplies the date hierarchy used for date drill-down.

## DAX Measures

The checked-in semantic model currently defines these measures:

- **Total Sales** — sums `Fact_Sales[sales_amount]`.
- **MoM Growth %** — compares current sales with sales from the previous month.
- **Running Total Sales** — calculates year-to-date sales using the date context.

The following measures are also specified for the project, but are not currently present in the checked-in semantic model definition:

- **Item Sales Rank** — ranks items by `[Total Sales]` in descending order.
- **Average Sale Value** — averages `Fact_Sales[sales_amount]`.

## Dashboard Features

- City sales comparison
- Cold Brew sales over time
- Product sales comparison
- City slicer for filtering the report
- Date hierarchy drill-down by year, quarter, month, and day

## Key Insights

Replace these placeholders with findings verified in the Power BI dashboard:

- **Top city by sales:** [Add verified city and result]
- **Sales trend for Cold Brew:** [Describe the verified pattern and period]
- **Top-selling product:** [Add verified product and result]
- **Month-over-month change:** [Add verified period and result]
- **Other notable observation:** [Add a dashboard-supported finding]
