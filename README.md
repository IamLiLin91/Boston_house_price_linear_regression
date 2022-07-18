# Boston_house_price_linear_regression
![image](https://user-images.githubusercontent.com/109471364/179448490-3e8cae0d-558b-4a98-8ba3-67bbff491eb2.png)

## Background
The Boston house price dataset contains information about the housing values in suburbs of Boston. This dataset was originally taken from the StatLib library which is maintained at Carnegie Mellon University and is now available on the UCI Machine Learning Repository. Each instance describes the properties of a Boston suburb and the task is to predict the house prices in thousands of dollars. There are 13 numerical input variables with varying scales describing the properties of suburbs. Read housing.names file before implementing your algorithm to check whether you need to do any data preprocessing steps. To give a brief introduction, the Boston housing data consists of 506 instances that represent the aggregated data about 14 features for homes from various suburbs in Boston. The input attributes and the output attribute are as follows:
1. CRIM: per capita crime rate by town
2. ZN: proportion of residential land zoned for lots over 25000 sq. ft.
3. INDUS: proportion of non-retail business acres per town
4. CHAS: Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)
5. NOX: nitric oxides concentration (parts per 10 million)
6. RM: average number of rooms per dwelling
7. AGE: proportion of owner-occupied units built prior to 1940
8. DIS: weighted distances to five Boston employment centers
9. RAD: index of accessibility to radial highways
10. TAX: full-value property-tax rate per $10,000
11. PTRATIO: pupil-teacher ratio by town
12. B: 1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town
13. LSTAT: % lower status of the population
14. MEDV (output): Median value of owner-occupied homes in $1000's

## Tasks
1. State whether you need to perform any data preprocessing on this dataset and do those preprocessing steps if needed.
2. Construct the linear regression equation to predict the housing prices in Boston. Explain this equation briefly and the number of parameters that need to be determined. 
3. Plot the input attributes (pick any 5 relevant attributes) and the output attribute in the given dataset to visualize how the output variable varies with respect to each of your input attribute.
4. Construct the Root Mean Squared Error (RMSE) function and R2-Score function using the linear regression equation that you constructed in task 2. Briefly explain these functions in your report. Implement RMSE and R2-Score functions in Python codes.
5. Describe briefly on the gradient descent learning algorithm for learning the parameters of your linear regression function. Implement it in Python codes. How are you going to find the optimal value of the learning rate (α)? Explain in this section.
6. Normalize the 13 input features by using equation: (data-min)/(max-min) . You can use the dataNorm() function you wrote in previous project.
7. Split the dataset into train (90%) and test (10%) using the splitTT function you built in previous project.
8. With train dataset, run the gradient descent algorithm to compute the parameters. Using these parameters, find and plot predicted_y_train VS actual_y_train , and predicted_y_test VS actual_y_test. What do you observe? In addition, using RMSE and R2-score, you are to evaluate on how accurate your model is.
9. Import from sklearn library and build a LinearRegression model (skeleton provided below, you are highly encouraged to read the official API) using the same train and test dataset you split in task 7. Compare the accuracy of your model and the sklearn model.
