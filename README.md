# Housing Rent Dynamics and Housing Supply in the Netherlands (2015–2025)

## 1. Introduction

As I prepare for my master's studies in the Netherlands, I became intrigued by the dynamics of the Dutch housing market. Rent levels in Dutch cities seemed persistently high, and I wondered what drives price changes. This analysis investigates how rent increases between 2015 and 2025 relate to changes in housing supply across regions in the Netherlands.

To achieve this, I conducted a data analysis project using official public data from Statistics Netherlands (CBS). The study focuses on two main components:

- Annual rent increases by region, including and excluding rent harmonisation  
- Annual changes in the housing stock (new construction, demolitions, and net additions)

This repository contains the full analysis, visualizations, and statistical findings.

---

## 2. Data Sources

This study uses official open-data from Statistics Netherlands (Centraal Bureau voor de Statistiek, CBS):

- **Rent Increase by Region (2015–2025)** – annual rent increase percentages including and excluding rent harmonisation, by region and major municipalities.  
- **Dwellings and Non-Residential Buildings: Stock and Changes (2012–2025)** – annual figures on total housing stock, new construction, demolitions, and net stock change by region.

Both CSV datasets are stored in the `data/` directory of this repository.

---

## 3. Research Questions

The analysis was guided by three primary questions:

1. How have rent prices evolved nationally and across major Dutch cities between 2015 and 2025?
2. How has the housing stock changed during the same period?
3. Is there a measurable relationship between changes in housing supply and annual rent increases?

---

## 4. Methodology

The analysis was performed in a Jupyter Notebook using Python. The main steps were:

## Data Loading and Cleaning
- Importing CSV datasets from CBS
- Standardizing region names
- Managing missing values
- Structuring the data into annual time series

## Exploratory Data Analysis
- Trends in national rent increases (2015–2025)
- Comparison of rent dynamics across Amsterdam, Rotterdam, The Hague, and Utrecht
- Annual housing stock growth by city
- Construction and demolition activity

## Visualisation
A series of plots was generated, including:
- Time-series line charts for rent trends
- City-level comparison plots
- Housing stock evolution graphs
- Heatmaps for rent intensity per city and year
- Dual-axis charts showing rent vs supply metrics

## Statistical Testing
To evaluate the relationship between supply and rents:
- Pearson correlation between rent increase and new construction
- Pearson correlation between rent increase and net stock change

Both tests were conducted at a 95% confidence level.

---

## 5. Key Findings

- **National Trends** – The average annual rent increase across the Netherlands from 2015 to 2025 was approximately 2.70%, with a low of 0.8% in 2021 and a high exceeding 5% in 2024.  
- **City Comparison** – Amsterdam recorded the highest average rent increase (~3.29%), followed by Rotterdam (~3.16%), The Hague (~2.88%), and Utrecht (~2.83%).  
- **Housing Supply** – The national housing stock grew by roughly 9.05% from 2015 to 2024 (+686,514 dwellings). Amsterdam led construction activity, while net additions were less consistent in other major cities.  
- **Correlation Results** – Year-to-year correlations between rent increases and both new construction (r = 0.143, p ≈ 0.693) and net stock change (r = 0.123, p ≈ 0.735) were not statistically significant, suggesting that short-term supply changes alone do not explain rent dynamics.


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

1. Clone the repository:  
   git clone https://github.com/IliasChristidisPlg/housing-rents-netherlands-analysis.git
2. Install dependencies:
   pip install -r requirements.txt
3. Open the notebook:
   jupyter notebook notebooks/analysis.ipynb
   
---


## 10. Conclusion

This analysis reveals that despite a significant increase in housing stock across the Netherlands, rent prices continued to rise, particularly in top cities like Amsterdam. The absence of a strong statistical link between annual supply changes and rent increases indicates that other factors—such as market regulation, inflation, or tenant turnover via rent harmonisation—play key roles. These findings provide insight into affordability pressures in the Dutch housing market and demonstrate applied data-analysis skills across multiple datasets and techniques.



