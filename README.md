# Real-Estate-Data-Analysis

**Overview**

Selling real estate plays a crucial role in the US economy, and understanding accurate pricing and the likelihood of a home selling is essential for comprehending the real estate market. This project explores the 
factors influencing home sales, with a focus on price and location. The research employs various models, highlighting the effectiveness of non-parametric tree-based models in conjunction with maps for predicting 
prices and determining home sales.

<br>

**Data Sources**

To conduct this analysis, the following datasets were utilized:

1. USA Real Estate Data Set (Zillow) - Kaggle
2. Buy vs Rent (Zillow) - Kaggle
3. Zip-Code-To-County - GitHub
4. US Zipcode to County State to FIPS lookup - Data.world
5. States.csv - Group-created file to facilitate data merging
6. Fips2County.tsv - GitHub

<br>

**Predictive Models**

<ol>
<li>For Predicting Prices</li>
<ul>
<li>Parametric Models:</li>
<br>
Linear Regression
Ridge and Lasso Regression - Implemented due to correlated independent variables, aiming for variable scaling/elimination.

<li>Non-parametric Models:</li>
<br>
Decision Tree: Regression decision tree
Random Forest: Regression-based random forest
</ul>
<li>For Sold/Not Sold Classification</li>
<ul>
<li>Parametric Models:</li>
<br>
Logistic Regression

<li>Non-parametric Models:</li>
<br>
Decision Tree: Classification
Random Forest: Classification
</ul>
</ol>

<br>

**Features Used for Prediction**

For predicting prices and classification of sold/not sold, the following features were considered:
<br> 
<ul>
  <li>bed</li>
  <li>bath</li>
  <li>acre_lot</li>
  <li>house_size</li>
  <li>breakeven</li>
  <li>new_build</li>
  <li>state</li>
<\ul>

<br>

**Maps**

Geo-coordinate plots were generated for better visualization:
<ol>
<li>Price Prediction Categories:</li>
<ul>
  <li>Less than $250,000</li>
  <li>$250,000 to $500,000</li>
  <li>$500,000 to $750,000</li>
  <li>$750,000 to $1,000,000</li>
  <li>$1,000,000 and above</li>
</ul>
<br>
<li>Sold/Not Sold Classification:</li><br>
Color-coded map based on the classification of sold and not sold properties.
</ol>

<br>

**Conclusion**

This real estate analysis project provides insights into the US real estate market, emphasizing the importance of price and location. The employed models, datasets, and visualizations contribute to a 
comprehensive understanding of factors influencing home sales and pricing.
