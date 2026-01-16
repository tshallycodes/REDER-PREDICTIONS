# Tshabron Telecoms Franchise Internship – Data Analysis with Python, SQL, and Tableau

## Overview
- Internship focused on **analyzing sales, expenses, and staff trends** for a telecoms franchise.
- Tools used: **Python (pandas, matplotlib, seaborn), SQL, Tableau**
- Goal: Provide actionable insights and recommendations to improve operational efficiency and profitability.

## Project Objectives
- Analyze **sales trends** across branches and products
- Identify **cost patterns** and areas for expense optimization
- Track **staff performance** and allocation
- Present findings using **interactive dashboards**
- Recommend **solutions to improve revenue and efficiency**

## Data Sources
- Sales reports per branch (Excel/CSV)
- Expense reports
- Staff logs and shift schedules
- Inventory and product data

## Key Tasks
### Data Collection & Cleaning
- Import data from CSV/Excel
- Handle missing values and inconsistencies
- Merge datasets for comprehensive analysis

### Data Analysis
- **Sales Analysis:** Total sales, monthly trends, product performance
- **Expenses Analysis:** Branch-wise and category-wise costs
- **Staff Analysis:** Productivity, attendance, allocation efficiency
- **Correlation Analysis:** Relationship between staff, sales, and expenses

### Visualization
- **Python/Matplotlib/Seaborn:** Exploratory plots for trends and correlations
- **Tableau Dashboards:** Interactive visualizations for stakeholders
    - Branch-wise sales comparison
    - Expense breakdown
    - Staff performance metrics

### Recommendations
- Optimize staffing based on peak sales hours
- Reduce unnecessary expenses per branch
- Promote high-selling products in underperforming locations
- Implement consistent reporting for better decision making

## Tools & Technologies
- **Python:** pandas, numpy, matplotlib, seaborn
- **SQL:** Data extraction, aggregation, and joins
- **Tableau:** Interactive dashboards and visual storytelling

## Outcomes
- Delivered actionable insights to **improve sales and efficiency**
- Provided **visual dashboards** for management to monitor key metrics
- Enhanced skills in **data cleaning, analysis, visualization, and reporting**

## Example Usage
```python
# Example: Summarize total sales per branch
import pandas as pd

sales_data = pd.read_csv("sales_report.csv")
branch_sales = sales_data.groupby("Branch")["Revenue"].sum()
print(branch_sales)
