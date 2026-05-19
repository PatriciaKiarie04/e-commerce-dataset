# E-Commerce Data Analysis Project

## Overview
Exploratory data analysis of an online retail dataset containing 1000 rows and 13 columns
covering customer behavior, product categories, payment methods, and satisfaction scores.

## Objectives
- Understand what customers are buying most
- Identify preferred payment methods
- Analyze customer demographics
- Measure overall customer satisfaction

## Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Google Colab

## Data Cleaning
- Identified and handled 103 missing values in the Gender column using mode imputation
- Identified and handled 201 missing values in the Review Score column using mean imputation
- Verified all missing values were resolved before analysis

## Key Findings

### 1. Sales by Category
Sports and Outdoors was the most purchased category with over 200 orders,
followed by Electronics and Fashion respectively.
This suggests the store's core customer base is active and lifestyle oriented.

### 2. Payment Method Analysis
Cash on delivery was the most preferred payment method with over 350 orders,
while credit card was the least used with approximately 300 orders.
This indicates customers may lack trust in online payment systems,
which presents an opportunity to build confidence through secure payment campaigns
or card payment incentives.

### 3. Customer Gender Distribution
Male customers placed slightly more orders than female customers with a difference
of approximately 50 orders. The relatively balanced gender split suggests the store
has broad appeal, however there is a clear opportunity to grow the female customer base
through targeted marketing strategies.

### 4. Review Score Distribution
Most review scores clustered around 4.0 with the distribution leaning negative,
indicating customers are moderately satisfied but not reaching loyal or delighted levels.
This suggests the business should investigate pain points preventing 5 star reviews,
such as delivery experience, product quality, or customer service.

## Business Recommendations
- Invest more inventory and marketing in Sports and Outdoors given its dominance
- Run trust building campaigns around online and card payments to reduce cash dependency
- Develop female targeted marketing campaigns to close the gender order gap
- Investigate and address the factors preventing customers from giving 5 star reviews

## Deeper Analysis Findings

### Age vs Spending
No strong relationship was found between age and spending.
Male customers showed slightly higher spending concentration across all age groups,
but overall spending is fairly random suggesting the store appeals broadly across ages.

### Age vs Review Score
Older customers tend to rate slightly higher than younger ones.
When grouped by age bracket, customers under 25, between 35-45 and above 55
were most satisfied while the 45-55 age group was least satisfied.
The overall difference between groups was small suggesting age is not
a strong driver of satisfaction.

### Price vs Review Score
No relationship was found between price and satisfaction.
Customers rate products similarly regardless of whether they cost $20 or $500,
meaning price alone does not drive customer satisfaction or dissatisfaction.

### Quantity vs Review Score
Customers ordering 3 items rated highest while those ordering 1 or 5 items
rated lower. This Goldilocks pattern suggests first time single item buyers
need a better onboarding experience while bulk buyers may be experiencing
delivery or fulfillment issues worth investigating.

## Business Recommendations
- Invest more inventory and marketing in Sports and Outdoors given its dominance
- Run trust building campaigns around online and card payments to reduce cash dependency
- Develop female targeted marketing campaigns to close the gender order gap
- Investigate and address factors preventing customers from giving 5 star reviews
- Improve first time buyer experience to convert single item purchasers into repeat customers
- Investigate fulfillment and delivery process for bulk orders of 5 or more items
- Focus satisfaction improvement efforts on the 45-55 age demographic

## Project Status
Exploratory analysis and deeper statistical analysis completed.
Next steps include predictive modeling using machine learning.
