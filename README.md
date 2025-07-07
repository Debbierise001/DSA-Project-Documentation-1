# DSA-Project-Documentation-1
Amazon Product Review Analysis

## Project Topic: Amazon Product Review Analysis for E-commerce Optimization

### Project Overview
This project explores Amazon product data using Microsoft Excel to analyze review patterns, pricing strategies, and discount performance across categories. The goal is to extract key insights that sellers and marketers can use to improve product placement, pricing models, and review engagement.

### Data Source
The dataset used for this project was provided by The Incubator Hub as an Excel file titled "Amazon Case Study.xlsx". It contains product information, pricing, ratings, and customer review counts sourced from Amazon pages for educational purposes.

### Tools Used
**Microsoft Excel** [Download Here](https://github.com/Debbierise001/DSA-Project-Documentation-1/blob/main/Amazon%20case%20study.xlsx)
- Data Collection
- Data Cleaning
- Calculations
  - Excel Formulas such as COUNT, IF, and COUNTIF
  - Calculated columns such as Discount %, Discount % >=50%, Potential Revenue, Price Bucket, and Composite Score.
    
- Summarization
  - Pivot Tables to aggregate and summarize insights
- Dashboard
  - Excel Charts and Pivot Charts to visualize trends and relationships
  - Tables to identify products with the highest average rating, highest ratings, e.t.c

### Data Cleaning & Preparation
- Removed unnecessary columns such as image link, product link, review content, review title, username, user ID, and review ID
- Shortened long product names to the first four words for clarity and consistency
- Added space to the category and removed other unwanted words.

### Calculations and Analysis
a. **Calculated columns**
- To measure how much each product was discounted
  - ```Discount% = (Actual Price - Discounted Price) / Actual Price * 100```
- To label products with discounts equal to or greater than 50%
  - ```Discount % >=50% =IF([@Discount%] >= 50, "Yes", "No")```
- To estimate revenue based on review count
  - ```Potential Revenue = Actual Price * Rating Count```
- To rank products by rating and popularity
  - ```Composite Score  =  Average Rating + (Rating Count / 1000)```
- To group discounts into ranges
  - ```Discount Bucket= IF([@Discount%]<=10, "0–10%", IF([@Discount%]<=20, "11–20%", ...))```
- To categorize prices into bands
  - ```Price Bucket = IF([@Discounted Price]<200, "<₹200", IF([@Discounted Price]<=500, "₹200–₹500", ">₹500"))```

b. **Pivot Tables**
- Analyzed average discount % and average prices by category.
- Counted the number of products and total reviews per category.
- Identified products with the highest ratings and most reviews.
- Summarized potential revenue per category.

![Pivot Table](https://github.com/Debbierise001/DSA-Project-Documentation-1/blob/main/Pivot%20Table.PNG)
![Pivot Table(Slicer)](https://github.com/Debbierise001/DSA-Project-Documentation-1/blob/main/Pivot%20Table(Slicer).PNG) 

c. **Dashboard**
- Built charts (bar, line, pie and column) to present results.

![Dashboard](https://github.com/Debbierise001/DSA-Project-Documentation-1/blob/main/Dashboard.PNG)
![Dashboard(Slicer)](https://github.com/Debbierise001/DSA-Project-Documentation-1/blob/main/Dashboard%20(Slicer).PNG)

### Trend & Relationship Analysis
- Compared rating patterns across discount ranges.
- Identified categories with highest discount rates.
- Ranked top products using combined rating and review score.

### Recommendation 
 - Focus should be on categories with the highest revenue potential.
 - Highly rated products with fewer reviews should be promoted.
 - 20–50% discounts should be used to boost mid-range product performance.
 - More products in the 200–500 price range should be developed.
 - Highlight products with strong ratings and review counts.
   
### Limitation 
- The dataset may not reflect real-time or complete Amazon product data.
- Limited data on user demographics or actual sales volume

### Reference 
- Dataset provided by training program
- Analysis done using Microsoft Excel
- Formulas and methods based on what was learned during the course
