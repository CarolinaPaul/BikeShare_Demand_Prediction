**Objective:**

* Understand the trends in the data and identify key factors affecting the hourly demand for rental bikes.
* Build an appropriate regression model to forecast the number of rental bikes required per hour

**Introduction**

A bike-sharing system is an innovative transportation strategy that provides individuals with bikes for their common use on a short-term basis for a price or for free. Over the last few decades, there has been a significant increase in the popularity of bike-sharing systems all over the world. This is because it is an environmentally sustainable, convenient, and economical way of improving urban mobility. In addition to this, this system also helps to promote healthier habits among its users and reduce fuel consumption.

**Conclusion:**

**Findings from EDA:**

* Temperature and Hour have a strong correlation with the count of rented bikes.
* Dew point temperature is highly positively correlated to the Temperature.
* Over the weekend and during holidays, rental bike demand decreases.
* There is a significant drop in the number of rented bikes during Winters(Dec-Feb) because it's freezing cold!
* The demand for bikes increases during warmer temperatures,which is why there's maximum count of rented bikes during the Summer season.
* In all seasons,the peak demands for rental bikes occur on the opening (8-9 AM) and closing times (6-7pm) of offices and institutions.

**Conclusion based on Model Evaluation:**

Calculated MAE, MSE, RMSE, and R2 scores for each model. Based on r2 score will decide the model performance.

Assumption: if the difference in R2 score between the Train data and the Test is more than 5 % we will consider it as overfitting.

* Gradient Boosting Regression(GridSearchCV) and Random forest gave good r2 scores. We can deploy any of these models.
* Temperature and Hour were found to be most influential variables in predicting the hourly demand for rental bikes
