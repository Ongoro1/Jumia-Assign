# Jumia-Assign
The Objective of this project is to design and build an interactive excel dashboard that analyzes products listed on jumia.
# Data Cleaning
The following steps were followed in data cleaning, missing values in rating and reviews columns were replaced by not provided bu using `control H`. in excel.
 
Duplicate products were removed by selecting all the data and using thr remove duplicate tab.

The rating,price and discount columns were converted into numericals.

Negatives were converted to positives using the absolute value in excel `abs`.
# Data Enrichment.
Additional calculated columns were added to enhance analysis.

Discount amount column was added by getting the values of `old price-new price`.

Rating category column was added by using the `if` formula in excel `=IF(J3="Not Provided", "Not Provided", IF(J3<3, "Poor", IF(J3<=4.4, "Average","Excellent")))`.

Discount Category column was added by using the `if` formula in excel `=IF(D2<20%, "Low", IF(D2<=40%, "Medium","high"))`
# Dashboard Design
A single interactive dashboard was created with the following sections;

## KPIs

* Total Number of products.
* Average Rating.
* Average discount percentage.
* Total number of reviews.

## Products performance
* Top products by rating
* Top products by numbers of reviews.
* Top products by Percentage.
## Trend Analysis.
* Discount percentage vs number of reviews.
* Rating vs Reviews.

