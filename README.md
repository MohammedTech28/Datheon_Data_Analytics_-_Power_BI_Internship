# Datheon Data Analytics & Power BI Internship

- **Name:** Mohammed A R
- **Register No:** 421125106073
- **Program:** B.Tech AI & Data Science, IFET College of Engineering
- **Application ID:** DT-2026-20R6F

## Project Overview
This repository contains my completed tasks for the Datheon Data Analytics & Power BI Internship. Each task is stored in its own folder with source code, data and findings.

## Tasks Completed

### Task 1: Exploratory Data Analysis (EDA) on Superstore Retail Sales
- **Folder:** `Task_1/`
- **Notebook:** `Task_1/Mohammed_Superstore_EDA.ipynb`
- **Dataset:** `Task_1/Sample - Superstore.csv`
- **Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook

**What was done**
- Data wrangling: missing-value profiling, duplicate removal, date parsing and Year-Month extraction
- Aggregated Sales and Profit by Product Category, Region and Customer Segment
- Analysed customer purchase volume, monthly seasonality, category-wise revenue and discount sensitivity
- Plotted monthly sales velocity and discount-vs-profit scatter plots
- Documented 5 annotated business findings and an executive summary in Markdown

**Key findings**
1. Revenue leadership and margin leadership differ across categories.
2. Sales are strongly seasonal, with a year-end peak.
3. Discounts of 20% and above push orders into net loss.
4. Some sub-categories (for example Tables) are loss-making despite healthy sales.
5. The top 20% of customers generate about 48% of revenue, and the Consumer segment contributes about 51% of sales.

### Task 2: Interactive Power BI Executive Sales & Profit Dashboard
- **Folder:** `Task_2/`
- **Files:** `Task_2/Mohammed_Superstore_Dashboard.pbix`, `Task_2/Mohammed_Superstore_Dashboard.pdf`, `Task_2/dashboard_preview.png`
- **Tools:** Power BI Desktop, DAX, Power Query
- **What was done:**
  - Cleaned the data in Power Query (date locale fix, junk rows and duplicates removed)
  - Modelled a star schema (Orders, DimCustomer, DimProduct, DimDate)
  - Wrote DAX measures: Total Sales, Total Profit, Total Orders, Profit Margin %, Sales LY, YoY Sales Growth %
  - Built a 3-page dashboard: KPI cards with monthly trend and slicers, regional and category treemaps, and a profitability matrix with conditional formatting
  - Exported the dashboard as PDF

**Key findings**
1. The business generated about 2.30M in sales and 286K in profit across about 5K orders, an overall profit margin of 12.5%.
2. Sales are seasonal: they dip to the lowest point in February and peak in November and December.
3. Copiers (about 55.6K), Phones (about 44.5K) and Accessories (about 41.9K) are the top profit-making sub-categories.
4. Paper and Labels have the highest margins (about 43% and 44%), even though their sales are small.
5. Tables (about -17.7K), Bookcases (about -3.5K) and Supplies (about -1.2K) are loss-making and need pricing or discount review.
6. The West region has the largest sales, followed by the East; Central and South trail behind.

## Repository Structure
```
Datheon_Data_Analytics_Power_BI_Internship/
├── README.md
├── Task_1/
│   ├── Mohammed_Superstore_EDA.ipynb
│   └── Sample - Superstore.csv
└── Task_2/
    ├── Mohammed_Superstore_Dashboard.pbix
    ├── Mohammed_Superstore_Dashboard.pdf
    └── dashboard_preview.png
```

## How to Run Task 1
1. Clone or download this repository.
2. Install the requirements:
   ```
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Open `Task_1/Mohammed_Superstore_EDA.ipynb` in Jupyter or VS Code.
4. Click **Run All**.

## How to Run Task 2
1. Install Power BI Desktop (free, Windows only).
2. Open `Task_2/Mohammed_Superstore_Dashboard.pbix` in Power BI Desktop.
3. Use the Year and Region slicers to explore the dashboard.
4. A PDF export is available at `Task_2/Mohammed_Superstore_Dashboard.pdf`.
