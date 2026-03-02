# Online Retail Sales Analysis

## Description

This project consists of an **online retail sales analysis** using a transactional dataset.  
The goal is to understand business performance, identify the most profitable products, categories, and markets, and provide **actionable business insights** to guide strategic decisions.

The dataset contains transactions with the following information: `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, and `Country`.


## Project Objectives

1. Identify the **most profitable products and categories**.  
2. Analyze **revenue distribution by country**.  
3. Study **sales trends over time** (weekly and monthly).  
4. Provide **practical recommendations** to improve profitability and reduce risks.


## Analysis Steps

###  Data Cleaning

- Removed missing `CustomerID`, duplicate transactions, negative quantities, and zero/negative prices.  
- Converted `InvoiceDate` to datetime format.  
- Created a `Revenue` column = `Quantity` × `UnitPrice`.  
- Created a `Category` column from product descriptions for category-level analysis.

**Insight:** After cleaning, the `df_clean` DataFrame contains only valid transactions, ensuring reliable results.


###  Product Analysis

- Calculated the **Top 10 revenue-generating products**.  
- Calculated the **percentage contribution** of these products to total revenue.

**Insight:** A small number of products generate a large share of total revenue.  
The company should focus **marketing and inventory management** on these high-performing items.


###  Category Analysis

- Calculated the **Top 5 most profitable categories** and their percentage contribution.

**Insight:** Certain categories dominate revenue. Prioritizing these categories for promotions and stock management can improve profitability.


###  Country Analysis

- Calculated the **Top 10 countries by revenue**.  
- Calculated each country’s share of total revenue.

**Insight:** Revenue is concentrated in a few key markets. Expanding into high-potential markets could **diversify revenue streams** and reduce risk.


###  Time Series Analysis

- Analyzed **monthly and weekly revenue** to identify trends and seasonality.

**Insights:**  
- Revenue shows **seasonal peaks** in certain months and weeks.  
- Marketing campaigns and inventory planning should be adjusted to **high-demand periods**.


## Business Recommendations

1. Prioritize **high-contributing products and categories** for marketing and inventory.  
2. Expand into **underexploited international markets** to diversify revenue.  
3. Plan campaigns and promotions **according to monthly and weekly revenue peaks**.  
4. Monitor **low-performing products or categories** for improvement or discontinuation.  
5. Diversify low-revenue products or markets to reduce dependence on top performers.


## How to Run the Code

1. Install dependencies:  

```bash
pip install pandas numpy matplotlib seaborn missingno