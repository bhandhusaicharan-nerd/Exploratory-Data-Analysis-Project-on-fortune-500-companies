# Fortune 500 India: Comparative Data Analysis (2022 vs 2025)

## 📌 Project Overview
This project performs an end-to-end Exploratory Data Analysis (EDA) comparing the financial performance and structural shifts of Fortune 500 companies between the years **2022** and **2025**. 

The analysis focuses on key financial metrics including Revenue, Net Profit, Assets, Debt-to-Equity, and Workforce efficiency.

## 🛠️ Technical Workflow

### 1. Data Acquisition & Cleaning
* **Source:** Web-scraped financial data from Fortune 500 rankings.
* **Multi-Index Handling:** Resolved complex multi-index headers and flattened column structures for analysis.
* **Regex Processing:** Used Regular Expressions (Regex) to split merged columns and clean non-numeric characters (currency symbols, commas).
* **Data Integrity:** Handled missing values and ensured correct data types (`int32`, `float64`) for 500+ records.

### 2. Statistical Analysis
* **Outlier Detection:** Used the **Interquartile Range (IQR)** method to identify and analyze market giants (statistical outliers).
* **Correlation Analysis:** Generated Pearson correlation matrices to understand the relationship between Revenue, Assets, and Headcount.
* **Comparative Growth:** Calculated Deltas (changes) in Revenue and Profitability over the 3-year period.

### 3. Key Visualizations
* **Capital Structure:** Stacked bar charts (Seaborn) visualizing the Debt vs. Net Worth ratio.
* **Market Concentration:** Pie charts illustrating the dominance of the Top 10 companies.
* **Workforce Trends:** Comparative histograms showing the shift in employee counts from 2022 to 2025.
* **Profitability Correlation:** Heatmaps showing the strength of relationships between different financial KPIs.

## 🚀 Key Insights
* **Revenue Concentration:** A significant percentage of total market income is held by the top 2% of companies.
* **Efficiency Gains:** Comparison of "Revenue per Employee" indicates a shift in corporate productivity over the last 3 years.
* **Leverage Trends:** Identified specific sectors that have significantly increased their Total Debt relative to Net Worth.

## 💻 Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook / Google Colab

## 📂 Project Structure
```text
├── data/               # Raw and Cleaned CSV files
├── notebooks/          # Final EDA Jupyter Notebook
├── scripts/            # Python scripts for data cleaning
└── README.md           # Project Documentation
