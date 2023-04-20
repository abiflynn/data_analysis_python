# Data Analysis: Is it Beneficial to Discount Products?

## 1. Project Objectives & Overview

 ### 1.1. Business Problem

Eniac is an online marketplace specialising in Apple-compatible accessories. It was founded 10 years ago in Spain, and it has since grown and expanded.

Working as a data analyst, I analysed the data to help resolve the ongoing debate on whether or not it’s beneficial to discount products.

- The Marketing Team Lead is convinced that offering discounts is beneficial in the long run. She believes discounts improve customer acquisition, satisfaction and retention, and allow the company to grow.

- The main investors in the Board are worried about offering aggressive discounts. They have pointed out how the company’s recent quarterly results showed an increase in orders placed, but a decrease in the total revenue. They prefer that the company positions itself in the quality segment, rather than competing to offer the lowest prices in the market.

### 1.2 Technical Skills

- Python 
- Pandas 
- Matplotlip
- Seaborn


## 2. Project Outcome 

### 2.1 Findings

**2.1.1 Eniac: Product Categories**

- Data Analysis based on completed orders only. 
- Classified the products into 19 categories
Top 5 Categories
1. Desktop - €3.0 mil
2. Other/ Misc - €2.9 mil 
3. Data Storage - €2.8 mil
4. Laptop - €2.5 mil
5. Monitor - €0.8 mil 
- A limitation of the data is that due to time constraints we have 1044 items that we were unable to manually categorise so we added them to a Other/Misc category. 
<img width="512" alt="Screenshot 2023-04-20 at 15 44 47" src="https://user-images.githubusercontent.com/120720780/233402211-3491f65d-9b71-407f-ad58-e417a7fde0fe.png">

**2.1.2 Eniac: Product Pricing Architecture**
- Average price of all products just under 500 euros, with a min and 2.99 euros and the max at just over 15,000 euros 
<img width="603" alt="Screenshot 2023-04-20 at 15 46 03" src="https://user-images.githubusercontent.com/120720780/233402586-552921bc-d176-4c69-87f7-7a300028489a.png">
- From the graph we can see there are two high value categories 
- And three categories with high value outliers 
- We can also see Desktop and Laptop  stand out as categories having a higher average price value vs other areas 

**2.1.3 Eniac: Discounts**
- 93.1% of all units sold were discounted (by 20.8 % on average) representing 95.0% of total revenue.
- High discounts do not directly result in high revenues, indicating they are not applied to high-value-products. 

General Effects of high discounts on low-value-products hard to assess:
- No data regarding stock-reduction
- No data on customers
- No data on shop-traffic

**2.1.4 Eniac: Seasonality**

<img width="670" alt="Screenshot 2023-04-20 at 15 49 25" src="https://user-images.githubusercontent.com/120720780/233403536-ecf11bb4-0632-420c-b18d-f78effd2f8ba.png">

- Reviewing total sales by month we can see strong peaks for black friday and strong sales in December for christmas
- As we have discounts all year round it looks like these peaks are driven by seasonality and not mainly by discounts 
- However looking at comparing Q1 sales for 2017 vs 2018 we can see that we have increased sales 
- This could be due to increased traffic over Black Friday and Xmas increasing market awareness
- With the data available I am not able to conclude if this is due to promotions


### 2.2 Recommendations 

**2.2.1 Limitations/ Data Collection Improvements** 

Unaware of the Company Goals: 
- Build Market Awareness E.g. Is there a need to drive increase traffic to site to build brand awareness? 
- Are they a new company? Trying to acquire the customer base

Missing Information:
- Profits / Cost Price / Margins
  - Although we can see peak in revenue we are unaware on how discounts are impacting company profits.

- Customer Information 
  - We do not have customer information therefore we cannot see if they are returning or being driven to the site with discounts.

Data Collection Improvements:

- Prices : To be rejected if entered incorrectly (with two decimals)
- Remove/ Reject Duplicates: When updating product-portfolio
- Datetime-Format: Automatically import date-inputs as datetime-format
- Column Names: Columns to have the same name if they contain the same information
- Database: Data to be in a Database not in 4 CSV files  

**2.2.2 It is Beneficial to Discount Products?** 

After cleaning and reviewing the dataset provided I am unable to advice if it is beneficial to discount products due to limitations in the data: 
1. Peaks in revenue are not mainly driven by discounts.
2. Assessing the beneficiality is difficult because we do not know the overall strategy of the company.
3. We are unaware of the impacts discounting is having on company profits. 
4. Since the dataset shows discounts over the whole time frame it’s not possible to assess what would happen if we were not discounting or only discounting on special occasions. 

