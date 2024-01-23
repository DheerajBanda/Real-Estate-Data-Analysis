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
Linear Regression<br>
Ridge and Lasso Regression - Implemented due to correlated independent variables, aiming for variable scaling/elimination.
<li>Non-parametric Models:</li>
Decision Tree: Regression decision tree<br>
Random Forest: Regression-based random forest
</ul>

<li>For Sold/Not Sold Classification</li>
<ul>
<li>Parametric Models:</li>
Logistic Regression
<li>Non-parametric Models:</li>
Decision Tree: Classification<br>
Random Forest: Classification
<br>
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
</ul>

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
<li>Sold/Not Sold Classification:</li>
Color-coded map based on the classification of sold and not sold properties.
</ol>

<br>

**Conclusion**

Based on the accuracy readings and model performance analysis, it is evident that non-parametric tree methods outperform parametric models in both predicting home prices and classifying homes that sell. The mean RSS (Residual Sum of Squares) for regression models and accuracy/misclassification for classification models were considered for evaluation.

<ol>
<li>Prediction of Home Prices</li>
<ul>
<li>Decision Tree and Random Forest models yielded lower mean RSS compared to parametric models (Regression, Ridge Regression, Lasso, GAM).</li>
<li>The location and price were identified as significant factors influencing the prediction of home prices.</li>
</ul>
  
<li>Classification of Homes that Sell</li>
<ul>
<li>Decision Tree and Random Forest models demonstrated higher accuracy in classifying homes that sell, outperforming Logistic Regression.</li>
<li>The classification matrix revealed that homes in the mid-price range (250,000 to 750,000) tended to sell more frequently.</li>
<li>Urban areas showed a higher likelihood of selling, aligning with the influence of location on home sales.</li>
</ul>

<li>Visualizing the Relationship</li>
To visualize the relationship between price and home sales, a matrix was created:<br>
<table>
  <tr>
    <th></th>
    <th>Sold</th>
    <th>Not Sold</th>
  </tr>
  <tr>
    <td>&lt;250k</td>
    <td>4221</td>
    <td>8351</td>
  </tr>
  <tr>
    <td>250k-500k</td>
    <td>10160</td>
    <td>7503</td>
  </tr>
  <tr>
    <td>500k-750k</td>
    <td>5407</td>
    <td>4378</td>
  </tr>
  <tr>
    <td>750k-1000k</td>
    <td>2854</td>
    <td>2410</td>
  </tr>
  <tr>
    <td>&gt;1000k</td>
    <td>4228</td>
    <td>4372</td>
  </tr>
</table>
This matrix highlights that mid-range priced homes (250,000 to 750,000) tend to sell more frequently. Additionally, homes located in urban areas are more likely to sell, which aligns with the observation that urban properties are generally priced higher. Therefore, homes listed in the range of 250,000 to 750,000 in urban areas are likely well-priced and have a higher chance of selling.<br>
In conclusion, the analysis emphasizes the significance of location and price in determining home sales. The decision tree models provide valuable insights into the interplay of these factors, contributing to a better understanding of the dynamics in the US real estate market.
</ol>
