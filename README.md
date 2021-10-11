# LINEAR REGRESSION

## What is linear regression?

Linear regression is a method for approximating a linear relationship between variables. While that may sound complicated, all it really means is that it takes some input variable, like the square footage of a house, and finds out how it's related to another variable, for example, the price it sells at.<br><br>
Linear Regression is used to predict the value of the dependent variable based on the values of other variables that impact it. 

## Simple Linear Regression

Simple linear regression means using one variable to predict a target variable. It is assumed that the two variables are linearly dependent, that is, if we plot input points on the x-axis and output points on the y-axis, they are linearly correlated. <br><br>
It uses the traditional slope-intercept form $y=mx+b$ where m and b are the variables our algorithm will try to 'learn' to produce the most accurate predictions. Here, x represents our input data, and y represents our prediction. The aim of linear regression is to find the line of best fit, which is the line that predicts the output variable with the minimum error. The line of best fit is also known as the regression line.<br><br>

### Example

For understanding simple linear regression better, we use common python libraries to model data and visualize the results.


This is an example of Simple Linear Regression using a data containing prices of cars and their various features.  <br><br>
We plot __*Price*__ against __*Horsepower*__. <br>This model is represented as *'Price ~ Horsepower'*<br><br>
From the scatter plot, we can see a strong linear relationship between these two variables. <br>
The red line, is the line our model predicted to summarize this relationship. This is the line of best fit.<br><br>
The equation of this line can be given by:<br>
$Price=-14607 +145.4*Horsepower$


![plot.png](attachment:plot.png)

To understand if the model is the best fit for the predictions, we can look at a number of parameters present in the model summary.

![summary.png](attachment:summary.png)

- Overall, we can see the model is a good fit to predict price as it has a high adjusted R-squared value at 0.575. Also, the probability value of the F statistic is very close to 0, and is less than 0.05 at a confidence level of 95%. <br>

- Horsepower is an important parameter to predict price as it p-value for the t-test is 0, which is less than 0.05 at a confidence level of 95%.<br>

- Horsepower positively impacts price. This means that for every unit increase in horsepower, the price increases by   $145.4.<br>


## Multiple Linear Regression

Unlike simple linear regression, multiple linear regression uses multiple variables to predict a target variable.<br><br>
An example of a multiple linear regression model is:<br>
*'price ~ Horsepower + Weight'* <br><br>

The equation of this line can be given by:<br>
$Price=-14607 +27.4*Horsepower + 9.5*Weight$

A multiple regressison model Multiple variables cannot be visualized in two-dimensional space. 

####  The implementation of the above example in python, is available above, in the 'Code' folder of the repository.
