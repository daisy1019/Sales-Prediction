# Blackwell Electronics Sales Prediction Report

**Introduction**

This report targets at the sales predictions for four product types: PC, Laptops, Netbooks and Smartphones for Blackwell Electronic to determine what type of products may impact sales across the enterprise.

The analysis is based on the following data features:

• Product / Price / Number of Star Reviews (x5, x4, x3, x2, x1)

• Type of reviews (Positive Service Review, Negative Service Review) • Recommend Product

• Shipping Weight / Width / Height / Depth

• Profit Margin

All these features were evaluated for sales Volume prediction for PC, Laptops, Netbooks and Smartphones.


**Analysis**

The correlation function was used to show the correlation relationship between features, the plot below shows that a strong positive correlation between sales volume and x5StarReviews, x4StarReviews and x3StarReviews, this also indicates that when Blackwell has better star reviews for these products, the sales volume is higher.

![CorrelationMatrix](https://user-images.githubusercontent.com/80385435/188295609-7281e569-7b53-4ea6-a4f8-9609085b52f5.png)

_Training Models Comparison_

Three training models were utilized to predict sales volume: Support Vector Machine(SVM), Random Forest(RF) and Stochastic Gradient Boosting(SGB).The execution time for predict the outcome was pretty close between these models, the SGB model was selected for prediction as it has lower RMSE and MAE score, while the Rsquared score is higher and it has the shortest training time.

  <img width="841" alt="Screen Shot 2022-09-03 at 8 21 55 PM" src="https://user-images.githubusercontent.com/80385435/188295689-3ec2c60b-55d4-4c24-b0de-4601f52be5c7.png">

_Variable Importance_

Variable Importance function was used to indicate the importance of each variable to Volume. Below graphs represent the variable importance result for using models SVM, RF and SGB. x5 / x4 / x3 /x2/ x1 / positive / negative start reviews are the more important features for predicted sales volume.

<img width="1107" alt="Screen Shot 2022-09-03 at 8 23 41 PM" src="https://user-images.githubusercontent.com/80385435/188295718-9210cec3-757f-4826-9bce-84573b24f763.png">

_Impact of reviews on sales volumes_

The following graphs exhibit the impact of reviews on sales volumes. The sales volume is higher with x5 / x4 and positive star reviews, the negative start reviews also predict higher sales volume for Netbook.

<img width="1168" alt="Screen Shot 2022-09-03 at 8 24 28 PM" src="https://user-images.githubusercontent.com/80385435/188295737-1ff890cb-556f-4bce-b778-aa97b4a137a2.png">


**Conclusions**

**• Potential business value learned from this analysis**

The potential business values from this analysis is that the customers’ reviews are an important factor for sales volume, Blackwell should maintain higher customers’ satisfaction rate for sales volume to increase.


**• Experience with rerun predictions of sales volume using both models**

It was straightforward to do so, however I encountered some errors and problems for training models and predicting sales outcome, all these was fixed by searching different online resources and seeking advice from mentors.


**• Recommendations for sales department relating to the different types of reviews**

Since reviews is the driven factor for higher sales volume, Blackwell should encourage customers to leave reviews if they are satisfied with the products that they purchased, even if they have problem with the product or the service, they should also leave reviews as negative reviews also drive the sales volume from previous graph that was presented. Blackwell can also reward customers with additional store credit or discounted future purchase if they leave reviews after their purchase.
