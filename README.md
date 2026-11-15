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

## Task 3: Customer Cohort & Churn Analytics

- **Folder:** `Task_3/`
- **Files:** `Task_3/churn_analysis.ipynb`, `Task_3/Customer_Churn_Dashboard.pbix`, `Task_3/Customer_Churn_Dashboard.pdf`, `Task_3/Churn_Analysis_Report.pdf`
- **Tools:** Python (pandas, Plotly), Power BI Desktop, DAX
- **What was done:**
  - Cleaned the IBM Telco Churn data (blank `TotalCharges` for new customers fixed) and created a churn flag
  - Calculated baseline churn rate and grouped customers into tenure cohorts (0-12, 13-24, 25-48, 49-60, 61-72 months)
  - Built the cohort retention matrix (contract type x tenure cohort) and retention curves by contract
  - Analysed churn by payment method, monthly charge band, and internet service with tech support
  - Wrote DAX measures: Total Customers, Churned Customers, Churn Rate %, Retention Rate %, Avg Monthly Charges
  - Built a 3-page dashboard: overview with KPI cards and slicers, cohort retention heatmap matrices, and churn drivers
  - Wrote a churn analysis report with retention recommendations and exported the dashboard as PDF

### Key findings

1. Overall churn is 26.54% (1,869 of 7,043 customers), so the retention rate is 73.46%.
2. The first year is the danger zone: customers with 0-12 months tenure churn at 47.44%, falling to 6.61% after five years. The first-year group makes up 55.5% of all churned customers.
3. Month-to-month contracts churn at 42.71% versus 2.83% for two-year contracts. New month-to-month customers (0-12 months) are the riskiest cohort at 51.35%.
4. Electronic check users churn at 45.29%, about three times the rate of customers paying automatically (15.24% to 16.71%).
5. Fiber optic customers without tech support churn at 49.37%, versus 22.63% with tech support. Fiber optic customers paying by electronic check churn at 53.23%.
6. Churn rises with price: the High monthly charge band churns at 37.51%, against 11.24% for the Low band.

### Retention recommendations

- Move month-to-month customers to one-year or two-year contracts with incentives.
- Build a first-year onboarding and engagement programme.
- Move electronic check users to automatic payment with a small discount.
- Bundle tech support with fiber optic plans.
- Run proactive retention outreach for fiber optic customers who pay by electronic check.
- Track the cohort retention matrix every month.

## Repository Structure
```
Datheon_Data_Analytics_Power_BI_Internship/
├── README.md
├── Task_1/
│   ├── Mohammed_Superstore_EDA.ipynb
│   └── Sample - Superstore.csv
├── Task_2/
│   ├── Mohammed_Superstore_Dashboard.pbix
│   ├── Mohammed_Superstore_Dashboard.pdf
│   └── dashboard_preview.png
└── Task_3/
    ├── churn_analysis.ipynb
    ├── Customer_Churn_Dashboard.pbix
    ├── Customer_Churn_Dashboard.pdf
    ├── Churn_Analysis_Report.pdf
    ├── Data/
    │   └── telco_customer_churn.csv
    ├── outputs/
    │   ├── telco_churn_clean.csv
    │   ├── churn_matrix.csv
    │   ├── retention_matrix.csv
    │   └── (8 interactive Plotly charts as HTML)
    └── Screenshot/
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

## How to Run Task 3

1. Clone or download this repository.
2. Install the requirements:

   ```
   pip install pandas numpy plotly jupyter ipykernel nbformat
   ```

3. Open `Task_3/churn_analysis.ipynb` in Jupyter or VS Code.
4. Click **Run All**. The cleaned data and interactive charts are saved in `Task_3/outputs/`.
5. Install Power BI Desktop (free, Windows only).
6. Open `Task_3/Customer_Churn_Dashboard.pbix` in Power BI Desktop. If it asks to refresh, point the data source to `Task_3/outputs/telco_churn_clean.csv`.
