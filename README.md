# Real-Estate-Data-Analysis

**Overview**

Selling real estate plays a crucial role in the US economy, and understanding accurate pricing and the likelihood of a home selling is essential for comprehending the real estate market. This project explores the 
factors influencing home sales, with a focus on price and location. The research employs various models, highlighting the effectiveness of non-parametric tree-based models in conjunction with maps for predicting 
prices and determining home sales.

**Data Sources**

To conduct this analysis, the following datasets were utilized:

1. USA Real Estate Data Set (Zillow) - Kaggle
2. Buy vs Rent (Zillow) - Kaggle
3. Zip-Code-To-County - GitHub
4. US Zipcode to County State to FIPS lookup - Data.world
5. States.csv - Group-created file to facilitate data merging
6. Fips2County.tsv - GitHub

**Predictive Models**

_For Predicting Prices_

Parametric Models:<br>
Linear Regression
Ridge and Lasso Regression - Implemented due to correlated independent variables, aiming for variable scaling/elimination.

Non-parametric Models:
Decision Tree: Regression decision tree
Random Forest: Regression-based random forest

_For Sold/Not Sold Classification_

Parametric Models:
Logistic Regression

Non-parametric Models:
Decision Tree: Classification
Random Forest: Classification

**Features Used for Prediction**

For predicting prices and classification of sold/not sold, the following features were considered:

<li>
  bed
  bath
  acre_lot
  house_size
  breakeven
  new_build
  state
<\li>

**Maps**

Geo-coordinate plots were generated for better visualization:

Price Prediction Categories:
<li>
  Less than $250,000
  $250,000 to $500,000
  $500,000 to $750,000
  $750,000 to $1,000,000
  $1,000,000 and above
  Sold/Not Sold Classification:
</li>

Color-coded map based on the classification of sold and not sold properties.

**Conclusion**
This real estate analysis project provides insights into the US real estate market, emphasizing the importance of price and location. The employed models, datasets, and visualizations contribute to a 
comprehensive understanding of factors influencing home sales and pricing.
