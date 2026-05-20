![Banner](banner.png)
# E-Commerce Data Analysis & Machine Learning Project

## Overview
End-to-end data science project analyzing an online retail dataset containing 
1000 rows and 13 columns. The project covers data cleaning, exploratory analysis, 
visualization, deeper statistical analysis, and a machine learning model to 
predict customer review scores.

## Objectives
- Understand what customers are buying most
- Identify preferred payment methods
- Analyze customer demographics
- Measure overall customer satisfaction
- Investigate relationships between age, price, quantity and review scores
- Build a machine learning model to predict customer satisfaction

## Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## Project Structure
1. Data Cleaning
2. Exploratory Data Analysis
3. Visualizations
4. Deeper Statistical Analysis
5. Machine Learning Model

---

## 1. Data Cleaning
- Loaded dataset of 1000 rows and 13 columns
- Identified 103 missing values in the Gender column and filled using mode imputation
- Identified 201 missing values in the Review Score column and filled using mean imputation
- Rounded review scores to whole numbers to prepare for machine learning classification
- Verified all missing values were resolved before proceeding to analysis

---

## 2. Exploratory Data Analysis & Visualizations

### Sales by Category
Sports and Outdoors was the most purchased category with over 200 orders,
followed by Electronics and Fashion respectively.
This suggests the store's core customer base is active and lifestyle oriented.

### Payment Method Analysis
Cash on delivery was the most preferred payment method with over 350 orders,
while credit card was the least used with approximately 300 orders.
This indicates customers may lack trust in online payment systems,
presenting an opportunity to build confidence through secure payment campaigns
or card payment incentives.

### Customer Gender Distribution
Male customers placed slightly more orders than female customers with a difference
of approximately 50 orders. The balanced gender split suggests broad appeal,
however there is a clear opportunity to grow the female customer base
through targeted marketing strategies.

### Review Score Distribution
Most review scores clustered around 4.0 with the distribution leaning negative,
indicating customers are moderately satisfied but not reaching loyal levels.
This suggests the business should investigate pain points preventing 5 star reviews
such as delivery experience, product quality, or customer service.

---

## 3. Deeper Statistical Analysis

### Age vs Spending
No strong relationship was found between age and spending.
Male customers showed slightly higher spending concentration across all age groups
but overall spending is random suggesting the store appeals broadly across all ages.

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

---

## 4. Machine Learning Model

### Goal
Predict a customer's review score based on their age, price paid, 
quantity ordered, and gender.

### Model Used
Random Forest Classifier with 100 decision trees.
A Random Forest works by building multiple decision trees and taking 
the most common prediction across all trees, making it reliable and 
robust for classification tasks.

### Process
- Encoded gender column from text to numbers using Label Encoder
- Defined inputs as age, price, quantity and gender
- Defined output as review score
- Split data into 80% training (800 rows) and 20% testing (200 rows)
- Trained model on training set and evaluated on unseen testing set

### Model Performance
- Overall Accuracy: 36.50%
- Best at predicting 4 star reviews with 0.43 precision and 0.52 recall
- Struggled with 1, 2 and 3 star reviews due to limited examples in dataset

### Confusion Matrix Findings
The model showed a strong bias toward predicting 4 and 5 star reviews
because those dominate the dataset. It correctly predicted 44 four-star 
reviews but struggled to identify dissatisfied customers giving 1, 2 or 3 stars.
This class imbalance is a key limitation of the current model.

### Why the Accuracy is 36.50%
Through our deeper analysis we discovered that age, price and quantity
have weak relationships with review scores. This means the features we 
provided do not strongly predict satisfaction. A stronger model would 
require additional features such as delivery time, return history, 
product category satisfaction, and customer lifetime value.

### Key Lesson
A machine learning model is only as good as the features provided to it.
This project demonstrates the importance of feature engineering and 
understanding your data before building models.

---

## Business Recommendations
- Invest more inventory and marketing in Sports and Outdoors given its dominance
- Run trust building campaigns around online and card payments to reduce cash dependency
- Develop female targeted marketing campaigns to close the gender order gap
- Investigate and address factors preventing customers from giving 5 star reviews
- Improve first time buyer experience to convert single item purchasers into repeat customers
- Investigate fulfillment and delivery for bulk orders of 5 or more items
- Focus satisfaction improvement efforts on the 45-55 age demographic
- Collect richer customer data including delivery time and return history
  to build a stronger predictive model in future iterations

---

## Limitations & Future Work
- Model accuracy of 36.50% indicates current features are weak predictors
- Class imbalance in review scores affects model performance on lower ratings
- Future iterations will include additional features and advanced models
  such as XGBoost or Neural Networks
- Sentiment analysis on customer reviews could provide stronger signals

## Project Status
✅ Data Cleaning
✅ Exploratory Data Analysis
✅ Visualizations
✅ Deeper Statistical Analysis
✅ Machine Learning Model
✅ Model Evaluation
✅ Business Recommendations

## Future Improvements
- Collect richer features such as delivery time, return history and 
  customer lifetime value to improve model accuracy
- Address class imbalance using oversampling techniques such as SMOTE
- Test advanced models such as XGBoost or Neural Networks
- Build an interactive dashboard using Tableau or Power BI
- Perform sentiment analysis on customer reviews for deeper satisfaction insights

## Author
- Data Science Undergraduate | Passionate about using data to drive 
  business strategy and decision making
- Tools: Python, Pandas, Matplotlib, Seaborn, Scikit-learn
- Currently exploring the intersection of Data Science, Business and AI
