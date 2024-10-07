# 📊 Financial Panel Dataset Analysis

This notebook provides a comprehensive analysis of a financial panel dataset through data exploration, feature engineering, model building, and evaluation. We'll examine the financial ratios and classification of various companies, extracting insights for further analysis.

## 📝 Table of Contents
1-Project Overview

2-Dataset Overview

3-Key Features Explained

4-Next Steps

5-Requirements

6-How to Run the Code

## 🧐 Project Overview.

This project demonstrates using a panel dataset to explore financial ratios across multiple companies. It covers everything from data exploration, and feature engineering, to model creation aimed at classifying companies based on their financial ratios.

## 📂 Dataset Overview

Entries: 2,570 records

Columns: 13 features

Unique Identifier: The code column represents different companies/entities.

Target Variable: Classification - a binary indicator (0 or 1) representing distinct categories for the companies  performance category).

The dataset is rich with financial ratios that help assess the companies' liquidity, profitability, valuation, and efficiency over time.

## 🛠️ Key Features Explained

•	code: A unique identifier for each company or entity in the dataset.
•	Classification: Binary classification column representing categories (e.g., financial status, health, or sector classification).
•	Current Ratio: Measures a company's ability to pay short-term obligations.
•	Quick Ratio: A more stringent liquidity measure, excluding inventories from current assets.
•	Cash Ratio: The ratio of cash and equivalents to current liabilities, showing liquidity strength.
•	Operating Cash Flow Ratio: Indicates how well cash flow from operations can cover liabilities.
•	Working Capital Ratio: The ratio of current assets to liabilities, revealing liquidity health.
•	Return On Equity (ROE): A profitability measure that reflects how much profit a company generates from shareholders' investments.
•	Net Profit Margin: The percentage of revenue left after all expenses are deducted from sales.
•	EBITDA: Earnings before Interest, Taxes, Depreciation, and Amortization, a measure of profitability.
•	EV/EBITDA: Enterprise Value to EBITDA ratio, used as a valuation metric.
•	EV / EBIT: The ratio of Enterprise Value to Earnings Before Interest and Taxes.
•	EV / Free Cash Flow: Shows how well a company generates cash relative to its valuation (Enterprise Value).
•	EV / Invested Capital: Reflects how well a company uses its invested capital.
•	EV / Revenue: Enterprise Value divided by total revenue, indicating valuation in terms of sales.
•	P/E Ratio: Price-to-Earnings ratio, a common valuation metric that compares a company's stock price to its earnings.
•	Price/Book: The ratio of a company's market value to its book value, used to assess whether a stock is undervalued or overvalued.
•	Dividend Per Share: The total dividends paid per share during a specific period.
•	Piotroski Score: A score evaluating financial strength, based on nine criteria related to profitability, leverage, and operational efficiency.

🧩 Next Steps
1. Data Exploration
Visualize and analyze trends, distributions, and relationships between features.
2. Feature Engineering
Derive new features that may improve model performance.
3. Model Building
Create and train classification models using financial ratios to predict company classifications.
4. Evaluation
Use accuracy, precision, recall, and other metrics to evaluate model performance.
📋 Requirements
Before running the notebook, ensure you have the following packages installed:

pandas
numpy
matplotlib
seaborn
scikit-learn
