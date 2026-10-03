# GitHub Copilot Notes

## 1. Total Sales

* **Copilot suggestion:** Used `SUM()` to calculate total sales.
* **Formula:** `SUM(Fact_Sales[sales_amount])`
* **Correction:** No correction needed.

## 2. Month-over-Month Growth

* **Copilot suggestion:** Used `CALCULATE()`, `PREVIOUSMONTH()`, and `DIVIDE()` to calculate monthly sales growth.
* **Correction:** No formula correction needed. Formatted the measure as a percentage.

## 3. Running Total Sales

* **Copilot suggestion:** Used `CALCULATE()` and `DATESYTD()` for year-to-date cumulative sales.
* **Correction:** No correction needed.

## 4. Item Sales Rank

* **Copilot suggestion:** Used `RANKX()` and `ALL()` to rank items by total sales in descending order.
* **Correction:** No correction needed.

## 5. Average Sale Value

* **Copilot suggestion:** Used `AVERAGE()` to calculate the average sales amount per fact-table row.
* **Correction:** No correction needed.

## Reflection

GitHub Copilot helped suggest DAX formulas and explain how each measure works. I reviewed the suggestions before entering them into Power BI and applied the required formatting. GitHub version control will help track changes and maintain the project history.
