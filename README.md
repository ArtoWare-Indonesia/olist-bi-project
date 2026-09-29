# Olist Brazilian E-Commerce — BI Analysis

## 1. Project Overview
This project analyzes the Olist Brazilian E-Commerce Public Dataset, a relational dataset from a Brazilian marketplace covering ~100k orders between 2016 and 2018. Unlike a single flat table, the dataset spans 9 linked tables, making it a practical exercise in data cleaning, data integration, and business analysis.

## 2. Business Problem
As a marketplace, Olist needs visibility into sales performance, customer satisfaction, seller performance, and delivery efficiency in order to identify operational improvements and growth opportunities.

## 3. Dataset
Source: [Olist Brazilian E-Commerce Public Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

9 tables: `orders`, `order_items`, `order_payments`, `order_reviews`, `customers`, `sellers`, `products`, `geolocation`, `product_category_name_translation`.

Raw CSV files are not included in this repository. Download them from the source above and place them in `data/raw/`.

## 4. Project Objectives
- Understand the structure and quality of all tables
- Clean and integrate data safely, respecting each table's grain
- Answer business questions on sales, customers, sellers, delivery, and reviews
- Translate findings into actionable business insights
- Build a BI dashboard from validated findings

## 5. Repository Structure
```
olist-bi-project/
├── README.md
├── requirements.txt
├── .gitignore
├── notebooks/
│   ├── v0.1.0_data_cleaning.ipynb
│   ├── v0.2.0_exploratory_analysis.ipynb
│   └── v0.3.0_advanced_analytics.ipynb
├── data/
│   ├── raw/
│   └── processed/
├── reports/
│   └── dashboard/
└── images/
```

## 6. Methodology
Understand → Clean → Analyze → Explain → Visualize → Dashboard

Tables are validated individually before joins. Merges are performed only at the grain required by each analysis to avoid row duplication.

## 7. Planned Analysis
- Sales by category, region, and time
- Delivery performance
- Delivery performance vs. review score
- Customer segmentation (RFM)
- Seller performance
- Geographic patterns

## 8. Dashboard
Planned for v0.4.0 using Power BI or Tableau, based on validated findings from the analysis.

## 9. Technologies
Python, pandas, numpy, matplotlib, seaborn, Jupyter Notebook, Git/GitHub, Power BI / Tableau.

## 10. How to Run
1. Clone this repository.
2. Create and activate a Python virtual environment.
3. Install dependencies: `pip install -r requirements.txt`.
4. Download the Olist dataset and place the CSV files in `data/raw/`.
5. Open the notebooks in GitHub Codespaces / VS Code and run them in order.

## 11. Project Roadmap
| Version | Focus |
|---|---|
| v0.1.0 | Data Cleaning & Data Integration |
| v0.2.0 | Exploratory Data Analysis |
| v0.3.0 | Advanced Analytics |
| v0.4.0 | Dashboard & Final Business Insights |

**Current status: v0.1.0 in progress.**
