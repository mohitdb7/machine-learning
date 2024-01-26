# Surprise Housing Case Study - Advance Regression
> Background
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below. The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.
The company wants to know:
Which variables are significant in predicting the price of a house, and How well those variables describe the price of a house. Also, determine the optimal value of lambda for ridge and lasso regression.
Business Goal
You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market..


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Model selection between Linear Regression, Ridge and Lasso
- Feature selection based on model
- Providing the effects of each feature on Sale Price of the hous

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
#### R2 Scores:
- -- Ridge Train score: 0.9343, Test score: 0.9171
- -- Lasso Train score: 0.9177, Test score: 0.9013
- -- Decision: Ridge has higher R2 Scores scores on both the training and test sets, indicating better overall predictive performance.
  
#### Mean Squared Error (MSE):
- -- Ridge Train MSE: 0.0098, Test MSE: 0.0134
- -- Lasso Train MSE: 0.0123, Test MSE: 0.0160
- -- Decision: Ridge has lower MSE on both the training and test sets, suggesting better accuracy in predicting the target variable.

#### Root Mean Squared Error (RMSE):
- -- Ridge Train RMSE: 0.0989, Test RMSE: 0.1159
- -- Lasso Train RMSE: 0.1108, Test RMSE: 0.1264
- -- Decision: Ridge has lower RMSE on both the training and test sets, indicating better accuracy and precision in predictions.

#### Considerations:
While both models seem to perform well, Ridge consistently outperforms Lasso across all metrics.
The choice between Ridge and Lasso can also depend on other factors such as interpretability (Lasso's tendency for feature selection) and the specific goals of your modeling.

#### Recommendation:
Though the R2 Score, MSE and RMSE of Ridge is better than Lasso but Lasso will generate a more simpler model as it has the capability of eleminating the features by setting them to zero.

- For a more simple model in terms of feature selection, choose Lasso.
- For a balance between simplicity and allowing all features to contribute, choose Ridge.

### Recommended Model - Lasso (for simpler model)

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python
- Pandas
- Numpy
- LinearRegression, Ridge, Lasso
- Scalling
- matplotlib.pyplot
- seaborn

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was developed as an assignment for Advance Regression


## Contact
Created by [@githubusername] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->