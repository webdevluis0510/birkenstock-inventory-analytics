# Birkenstock USA Inventory & Sales Analytics

**Status:** Complete | **Level:** Beginner  
**Author:** Luis  
**Date:** April 2026  

SQL-based retail analytics project analyzing inventory performance, sales trends, and supply chain efficiency for a Birkenstock USA store location using Python and SQLite.

---

## Project Overview

This project uses SQL and Python to analyze synthetic retail data modeled after real Birkenstock USA store operations. As a current stock lead at Birkenstock, I designed this project around actual inventory challenges I encounter on the floor daily, including dead stock management, size availability gaps, seasonal demand patterns, and supply chain timing issues.

---

## Business Questions Answered

1. Which styles generate the most revenue?
2. Which gender category drives the most sales?
3. Which styles have the highest dead stock?
4. Which sizes are most frequently understocked?
5. Which incoming shipments arrived in the wrong season?

---

## Key Findings

1. Arizona led all styles with 742 units sold and $75,387 in revenue, nearly double the second highest style (Gizeh at $39,129).

2. Womens category generated $139,430 in revenue, accounting for the overwhelming majority of sales compared to Mens ($43,145) and Kids ($6,090).

3. Naples averaged 114 days in stock, far exceeding all other styles. As a discontinued style, it represents significant dead stock tying up floor and stockroom space.

4. Six styles were flagged as understocked based on low average quantity and fast turnover. Boston averaged only 8 units per size heading into its peak Fall/Winter season.

5. 5 out of 10 incoming shipments (50%) arrived in the wrong season. All five were Fall/Winter styles arriving in April during peak Spring/Summer selling season.

---

## Tech Stack

- Python 3.x
- SQLite3 (database engine)
- Pandas (data manipulation)
- Matplotlib (visualization)
- Seaborn (visualization)
- Jupyter Notebook (development environment)

---

## Project Structure
birkenstock-inventory-analytics/
├── notebooks/
│   └── birkenstock_analytics.ipynb
├── data/
├── outputs/
├── .gitignore
├── requirements.txt
└── README.md

## Database Schema

Four tables were created to model store operations:

- Products: All Birkenstock styles, materials, gender, price, category, season, discontinued status
- Inventory: Stock levels per style and size, quantity on hand, reorder points, days in stock
- Sales: Transaction records from January to April 2026, sale dates, prices, sizes sold
- Shipments: Incoming stock records including expected vs actual arrival dates and season status

---

## Installation

```bash
git clone https://github.com/webdevluis0510/birkenstock-inventory-analytics.git
cd birkenstock-inventory-analytics

python -m venv venv
venv\Scripts\activate

pip install -r requirements.txt
```

Open notebooks/birkenstock_analytics.ipynb and run all cells in order. The database is generated automatically on first run.

---

## What I Learned

- Writing SQL queries (SELECT, JOIN, GROUP BY, HAVING, CASE WHEN)
- Creating and managing a SQLite database with Python
- Connecting Pandas DataFrames to SQL tables
- Generating synthetic datasets modeled after real world operations
- Translating business questions into SQL queries
- Visualizing SQL query results with Matplotlib and Seaborn
- Applying retail domain knowledge to data analysis

---

## Potential Improvements

- Connect to real Birkenstock POS system data for more accurate insights
- Expand dataset to cover multiple store locations and full year data
- Build size level analysis to pinpoint exact sizes needing replenishment
- Automate purchase order generation when stock drops below reorder point
- Add supplier performance tracking to shipments table
- Connect directly to Power BI for interactive real time dashboard

---

## Related Projects

- F1 Lap Time Analyzer - https://github.com/webdevluis0510/f1-lap-analyzer
- F1 Qualifying Performance Predictor - https://github.com/webdevluis0510/f1-qualifying-predictor

---

## Career Context

This project is part of my structured portfolio building toward a career as an MLOps Engineer.

Current Phase: Data Analyst portfolio (Python, SQL, Power BI, Excel)
Next Phase: DevOps track, AWS Solutions Architect, CompTIA Network+
Goal: Junior MLOps Engineer / Platform Engineer

---

Luis - https://github.com/webdevluis0510