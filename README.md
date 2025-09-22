## Project Title
Revenue-Returns-Monitor

## Brief One Line Summary
An end-to-end analytics dashboard diagnosing revenue drivers and profitability levers across products and markets.

## Overview
This project provides a structured business intelligence solution designed to address leadership blind spots in revenue performance. By consolidating multi-market sales data and applying diagnostic analytics, the solution highlights which categories, products, and geographies are truly driving profitability. The ultimate goal is to enable executive stakeholders to make evidence-based decisions on resource allocation and portfolio restructuring.  

The intended audience includes C-level executives, finance directors, category managers, and product strategy teams. The deliverable is a dynamic dashboard that surfaces high-value KPIs—revenue contribution, margin analysis, category growth trends—while allowing interactive slicing by market or product.  

The scope of this project goes beyond visualization: it incorporates systematic data cleaning, engineered profitability metrics, and governance-ready documentation. Deliverables include reproducible ETL pipelines, a monitoring dashboard, and a lightweight runbook for future iterations.

## Problem Statement
The business has a wide product portfolio, but it’s not clear which categories and products are truly driving profitability. As they look to restructure, leadership needs clarity on where to focus resources for maximum impact across different markets. 

## Tools and Technologies
- **Languages:** Python 3.11, SQL (MySQL 8.0)  
- **Libraries:** pandas, numpy, matplotlib, seaborn, plotly, scikit-learn  
- **Visualization:** Power BI, Streamlit (for lightweight prototype)  
- **Database:** MySQL, SQLite (for local testing)  
- **Workflow & Containerization:** Docker, Airflow (optional for orchestration)  
- **Version Control:** Git/GitHub  

## Methods
1. **Data Ingestion**  
   - Imported sales, product, and market data from CSV/SQL sources.  
   - Established schema alignment (standardized product IDs, date formats).  

2. **Data Cleaning**  
   - Removed duplicates and outliers.  
   - Imputed missing values with median (numeric) and mode (categorical).  

3. **Feature Engineering**  
   - Derived gross margin %, contribution margin per SKU.  
   - Created category-level revenue share metrics.  
   - Engineered rolling averages for demand volatility tracking.  

4. **Exploratory Data Analysis (EDA)**  
   - Revenue concentration curves (Pareto principle validation).  
   - Market-wise profitability segmentation.  
   - Product lifecycle visualization.  

5. **Validation & Stress Testing**  
   - Cross-validated profitability figures against finance-provided control data.  
   - Performed sensitivity analysis on margin assumptions.  

6. **Dashboard Development**  
   - Built Power BI report with drill-through functionality.  
   - Deployed a lightweight Streamlit prototype for rapid iteration.  

7. **Evaluation Metrics**  
   - % revenue from top categories.  
   - % products below profitability threshold.  
   - [REPLACE_WITH_ACTUAL_METRIC] from evaluation script (`python src/eval.py`).  

## Key Insights
- Apparel, Books, and Electronics are core revenue categories, but Electronics is more regionally volatile.
- Return rates are driven not just by percentages but by order volume (e.g., Nigeria had most returns due to high sales volume despite moderate return rates).
- Longer delivery times correlate directly with higher return rates (statistically significant at p < 0.05).
- Products like Books and Groceries have lower cost ratios, making them more profitable per unit compared to high-cost items like Laptops.
- Seasonal spikes (especially in December) create opportunities for targeted campaigns.

## Results & Conclusion

Prioritize investment in Apparel, Books, and regional Electronics markets (like Brazil).

Streamline logistics for deliveries >7 days to reduce return rates and improve profitability.

Investigate data inconsistencies between pivot tables and dashboard — ensure executives make decisions on the full dataset.

Double down on high-margin products (Books, Groceries) and leverage volume from low-margin but popular items (Electronics).

Plan seasonal promotions around Q4 to capitalize on proven spikes in demand.

## Author & Contact

Sahil Sahu
Data Analyst 
Email: your_email@example.com
