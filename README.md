# Housing Rent Dynamics and Housing Supply in the Netherlands (2015–2025)

## 1. Introduction

As part of my preparation for pursuing a master’s degree in the Netherlands, I became interested in understanding the country’s housing market. The frequent discussion about high rent levels, especially in major Dutch cities, motivated me to investigate how rents have evolved over the past decade. My goal was to identify patterns, quantify trends, and examine whether changes in housing supply have had a measurable impact on rent increases.

To achieve this, I conducted a data analysis project using official public data from Statistics Netherlands (CBS). The study focuses on two main components:

- Annual rent increases by region, including and excluding rent harmonisation  
- Annual changes in the housing stock (new construction, demolitions, and net additions)

This repository contains the full analysis, visualizations, and statistical findings.

---

## 2. Data Sources

All datasets used in the project come from the official CBS StatLine platform:

1. **Rent Increase by Region (2015–2025)**  
   Includes annual rent increase percentages, with and without harmonisation, for all Dutch regions and major municipalities.

2. **Dwellings and Non-Residential Buildings: Stock and Changes (2012–2025)**  
   Contains yearly data on:
   - Total housing stock
   - New construction volumes
   - Demolitions
   - Net stock change

Both datasets are included in the `/data` directory.

---

## 3. Research Questions

The analysis was guided by three primary questions:

1. How have rent prices evolved nationally and across major Dutch cities between 2015 and 2025?
2. How has the housing stock changed during the same period?
3. Is there a measurable relationship between changes in housing supply and annual rent increases?

---

## 4. Methodology

The analysis was performed in a Jupyter Notebook using Python. The main steps were:

### 4.1 Data Loading and Cleaning
- Importing CSV datasets from CBS
- Standardizing region names
- Managing missing values
- Structuring the data into annual time series

### 4.2 Exploratory Data Analysis
- Trends in national rent increases (2015–2025)
- Comparison of rent dynamics across Amsterdam, Rotterdam, The Hague, and Utrecht
- Annual housing stock growth by city
- Construction and demolition activity

### 4.3 Visualisation
A series of plots was generated, including:
- Time-series line charts for rent trends
- City-level comparison plots
- Housing stock evolution graphs
- Heatmaps for rent intensity per city and year
- Dual-axis charts showing rent vs supply metrics

### 4.4 Statistical Testing
To evaluate the relationship between supply and rents:
- Pearson correlation between rent increase and new construction
- Pearson correlation between rent increase and net stock change

Both tests were conducted at a 95% confidence level.

---

## 5. Key Findings

### 5.1 Rent Trends
- The national average rent increase during 2015–2025 was 2.70%.
- The lowest increase occurred in 2021 (0.8%), partly influenced by COVID-19 policy restrictions.
- The highest spike occurred in 2024 (above 5%).
- Amsterdam consistently showed the highest rent increases among major cities.

### 5.2 Housing Supply
- The national housing stock grew from 7.58 million dwellings in 2015 to 8.27 million in 2024 (+686,514 units).
- Amsterdam had the largest construction activity and the highest net stock gains.
- Rotterdam and The Hague showed moderate but less consistent housing expansion.
- Demolitions were significantly lower than new construction in all cities.

### 5.3 Correlation Analysis
- Rent Increase vs New Construction: correlation = 0.143 (not statistically significant)
- Rent Increase vs Net Stock Balance: correlation = 0.123 (not statistically significant)

This indicates that year-to-year fluctuations in housing supply do not have a measurable short-term impact on rent increases within this dataset.

---

## 6. Interpretation

The analysis suggests that although the Dutch housing stock has grown steadily over the past decade, this expansion has not been sufficient to stabilise rent increases. Rent dynamics appear to be influenced more by factors such as inflation, regulatory changes, harmonisation adjustments, and market tension rather than by annual changes in supply.  

In highly demanded cities like Amsterdam and Rotterdam, rent increases remain structurally higher, despite above-average construction activity.

---

## 7. Repository Structure

/
│── data/ # CBS datasets (CSV)
│── figures/ # Visualizations exported during analysis
│── notebooks/ # Jupyter Notebook with full analysis (analysis.ipynb)
│── outputs/ # Additional charts and processed visuals
│── README.md # Project documentation

---

## 8. Tools and Technologies

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  
- Git & GitHub  

---

## 9. How to Reproduce the Analysis

Clone the repositor: https://github.com/IliasChristidisPlg/housing-rents-netherlands-analysis.git

Install dependencies:pip install -r requirements.txt

Open the notebook:jupyter notebook notebooks/analysis.ipynb


---

## 10. Conclusion

This project provides a data-driven overview of the Dutch housing market over a decade. It highlights the strong upward trend in rents and demonstrates that short-term changes in housing supply alone are not sufficient to moderate price growth. The findings offer insight into the challenges of affordability in the Netherlands and reflect broader structural issues in the housing market.

The analysis also serves as a demonstration of applied data analysis skills, including data wrangling, time series exploration, statistical evaluation, and visual communication.


