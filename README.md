# Electric Vehicle Population Analysis — Washington State

> **Capstone Project | Exploratory Data Analysis & Visualization**  
> A deep dive into EV adoption patterns, manufacturers, and trends using real-world government data from Washington State.

---

## Project Overview

This project analyzes the **Electric Vehicle (EV) population in Washington State** to uncover patterns in EV adoption, distribution, and characteristics. Using a dataset of **276,828 vehicles** sourced from the U.S. Government Open Data Portal, this analysis applies end-to-end data science techniques — from cleaning and preprocessing to rich visual storytelling.

---

## Dataset

| Detail | Info |
|--------|------|
| **Source** | [U.S. Government Open Data Portal (Data.gov)](https://catalog.data.gov/dataset/electric-vehicle-population-data) |
| **Maintained by** | Washington State Department of Licensing |
| **Total Records** | 276,828 rows × 16 columns |
| **Key Columns** | County, City, Model Year, Make, Model, EV Type, Electric Range, Electric Utility |

---

## Analysis Focus

- Distribution of EVs across **counties and cities**
- Most popular **EV manufacturers and models**
- **EV adoption trends** by model year (1998–2026)
- Comparison of **BEV vs PHEV** types
- Variation in **electric range** across models and manufacturers

---

## Tools Used

Python
Pandas
Matplotlib
Seaborn
Plotly
Jupyter

---

## Visualizations Included

| # | Chart | Purpose |
|---|-------|---------|
| 1 | Histogram + KDE | Electric Range Distribution |
| 2 | Boxplot | Outlier Detection in Electric Range |
| 3 | Count Plot | EV Type Distribution (BEV vs PHEV) |
| 4 | Bar Chart | Top 10 EV Manufacturers |
| 5 | Bar Chart | Top 10 Electric Utilities |
| 6 | Bar Chart | Vehicle Age Group Distribution |
| 7 | Violin Plot | Electric Range by EV Type |
| 8 | Line Chart | EV Growth Over Years |
| 9 | KDE Plot | Electric Range Density |
| 10 | Scatter Plot | Electric Range vs Model Year |
| 11 | Pie Chart | EV Type Share |
| 12 | Line Chart | Average Electric Range by Year |
| 13 | Bar Chart | Top 10 Cities by EV Count |
| 14 | Plotly Bar | Average Range by Manufacturer (Interactive) |
| 15 | Stacked Bar | EV Count by Year & Type |
| 16 | Grouped Bar | Average Range by Make & EV Type |
| 17 | Line Chart | EV Type Distribution Over Model Years |
| 18 | Line Chart | Top 5 EV Makes Over Model Years |
| 19 | Heatmap | Numeric Feature Correlations |
| 20 | Line Chart | Cumulative EV Growth Over Years |

---

## Key Insights

### Adoption & Growth
- Minimal adoption from **2000–2007** (under 100 vehicles/year)
- Exponential surge from **2008 onwards**, with a major jump in **2020** (~174,687 cumulative)
- Growth peaked in **2023** with over 50,000 BEVs registered in a single year

### EV Types
- **BEVs dominate at ~80%** of the dataset (~221,329 vehicles)
- PHEVs account for ~20% with lower, more concentrated electric ranges

### Manufacturers & Range
- **Tesla leads** with 110,000+ vehicles — far ahead of Chevrolet, Nissan, Ford
- Tesla, Jaguar, and Polestar have the **highest average electric range (~240–250 miles)**
- Most vehicles fall in the **20–50 mile range**, with a secondary peak at 200–250 miles

### Geography
- **Seattle** has the highest EV count (~42,000), followed by a steep drop in other cities
- **Puget Sound Energy Inc** is the dominant electric utility serving EV owners

---

## Data Preprocessing Steps

1. **Column Renaming** — Standardized names (e.g., `VIN (1-10)` → `VIN`)
2. **State Name Standardization** — `'WA'` → `'WASHINGTON'`
3. **Invalid Range Removal** — Filtered out rows where `Electric_Range == 0`
4. **Missing Value Handling** — Categorical → `'Unknown'`; Numeric → mode/mean
5. **Duplicate Removal** — 0 duplicates found
6. **Data Type Correction** — Model Year → `int`, Electric Range → `float`
7. **Derived Column** — `Vehicle_Age = 2026 - Model_Year`
8. **Outlier Detection** — IQR method on valid Electric Range values
9. **Text Standardization** — Make/Model/State formatted consistently

---

## Project Structure

```
Capstone_Project-EDA___Visualization
 ┣ README.md                                     
 ┗ data/
    ┗ ElectricVehicle_Population_Data.csv          
```


## Relevance of the Topic

Electric vehicles play a critical role in **reducing carbon emissions** and promoting **sustainable transportation**. Understanding EV adoption patterns helps inform future infrastructure planning, policy decisions, and sustainable mobility solutions — making this both a technically rich and socially relevant analysis.

---

## Author

**Aiswarya P V**  
aiswaryaaswin1999@gmail.com  
🔗 [LinkedIn](www.linkedin.com/in/aiswaryapv) | [GitHub](https://github.com/aiswaryapv1999)

