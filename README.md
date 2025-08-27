# Project--AMAZON-sales-performance-
1. Introduction
From the accessible sales dataset, which contains information on product categories, sizes, fulfillment strategies, quantities sold, pricing, and customer types (B2B/B2C), the project's objective is to extract actionable insights. Optimizing operations, marketing, and sales strategies will be made easier with an understanding of trends in buyer behavior, fulfillment efficiency, and product performance.

2. Data sources use:
   	https://www.kaggle.com/datasets/thedevastator/unlock-profits-with-e-commerce-sales-data/data
   Data descriptions:

This dataset provides detailed insights into Amazon sales data, including SKU Code, Design Number, Stock, Category, Size and Color, to help optimize product profitability

Category: Type of product. (String)
Size: Size of the product. (String)
Date: Date of the sale. (Date)
Status: Status of the sale. (String)
Fulfilment: Method of fulfilment. (String)
Style: Style of the product. (String)
SKU: Stock Keeping Unit. (String)
ASIN: Amazon Standard Identification Number. (String)
Courier Status: Status of the courier. (String)
Qty: Quantity of the product. (Integer)
Amount: Amount of the sale. (Float)
B2B: Business to business sale. (Boolean)
Currency: The currency used for the sale. (String)

   
3. Initial Analysis Plan
   
 A. Data Cleaning
•	Handle missing values:
o	Fill categorical fields (e.g., currency, ship-country) with the most frequent values or appropriate placeholders ('Unknown', 'Not Provided').
o	Address numerical nulls (ship-postal-code) using median or zero where appropriate.
•	Standardize data types:
o	Convert Date column to datetime format.
o	Ensure numerical columns (Qty, Amount) are properly typed.
o	Remove or rename unnamed columns.
•	Remove duplicates and check for inconsistent entries (e.g., negative quantities or amounts).

 B. EDA
•	Univariate analysis:
o	Distribution of Qty, Amount, Category, Currency, and B2B.
•	Bivariate analysis:
o	Sales performance (Amount) by Category, Size, Style, Fulfilment, and B2B to Identify the best-selling product cateogry combinations.
•	Top best selling product
•	Top city AMZ do best selling
o	Trend analysis over Date (time series of sales volume and value).
•	Outlier detection:
o	Identify anomalies in sales quantity or amount (e.g., extremely high or low).

 C. Deeper Analysis
•	Segmentation:
o	Segment sales by B2B vs B2C, Category, and Fulfilment type.
•	Performance metrics:
o	Average revenue per SKU, top-selling products, top categories.
•	Fulfillment & logistics:
o	Analyze delivery performance based on Courier Status.
•	Currency conversion (optional):
o	Normalize Amount across currencies if needed for global analysis.

 D. Data Storytelling & Visualization
•	Use clear charts and narratives to communicate:
o	Sales trends and seasonality
o	Best-selling and underperforming products
o	Impact of fulfillment method on delivery and customer satisfaction
o	Insights into B2B vs B2C dynamics
 
 results 
•	Cleaned and structured dataset
•	Interactive EDA dashboard or notebook
•	Insightful visualizations and summary report
•	Strategic recommendations based on findings


