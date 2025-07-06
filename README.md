m# DSA-Project-Documentation-1
Amazon Product Review Analysis

## Project Topic: Amazon Product Review Analysis for E-commerce Optimization

### Project Overview
This project explores Amazon product data using Microsoft Excel to analyze review patterns, pricing strategies, and discount performance across categories. The goal is to extract key insights that sellers and marketers can use to improve product placement, pricing models, and review engagement.

### Data Source
TThe dataset used for this project was provided by The Incubator Hub as an Excel file titled "Amazon Case Study.xlsx". It contains product information, pricing, ratings, and customer review counts sourced from Amazon pages for educational purposes.

### Tools Used
- Microsoft Excel [Download Here]
  - Data Collection
  - Data Cleaning
  - Calculations
    - Formula such as COUNT
    - Calculated columns
  - Summarization
    - Pivot Tables to aggregate and summarize insights
  - Dashboard
   - Excel Charts to visualize trends and relationships
   - Tables to identify products with highst average rating, highest ratings e.t.c

### Data Cleaning & Preparation
- Removed unnecessary columns such as image link, product link, review content, review title, username, user ID, and review ID
- Shortened long product names to the first four words for clarity and consistency
- Added space to the category and remove other unwanted words.

### Calculations and Analysis
  #### **Calculated columns**
- To measured how much each product was discounted
  - ```Discount % = (Actual Price - Discounted Price) / Actual Price * 100```
- To labeled products with discount equal or greater than 50%
  - ```Discount % >50% =IF([@Discount%] >= 50, "Yes", "No")```
- To estimated revenue based on review count
  - ```Potential Revenue = Actual Price * Rating Count```
- To ranked products by rating and popularity
  - ```Composite Score  =  Average Rating + (Rating Count / 1000)```
  
  #### **Pivot Tables**
  - Analyzed average discount % and average prices by categor
  - Counted number of products and total reviews per category
  - Identified products with highest ratings and most reviews
  - Summarized potential revenue per category

  #### **Dashboard**
  - Built charts (bar, line, piechat and column) to present results

### Trend & Relationship Analysis
- Compared rating patterns across discount ranges
- Identified categories with highest discount rates
- Ranked top products using combined rating and review score
