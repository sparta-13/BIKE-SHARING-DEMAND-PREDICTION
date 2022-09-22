# Bike Sharing Demand Prediction
In this study, we aim to create a predictive model, which could be used to predict how many bike rentals will occur based on weather conditions throughout the year.  As a result, predictions can be made more quickly and efficiently.

Programming Language : Python

Libraries used : Pandas, Numpy, Matplotlib, Seaborn, Sklearn

NoteBook : Google Colab

Dataset Source : Provided by Almabetter themself.
## Objective
We are provided with a Seoul Bike Dataset. The main objective is to build a predictive model on the given dataset, which could help to train a model to predict the number of bike rentals of the year given the weather conditions.
## Dataset 
This dataset contains bike usage patterns with the weather data to forecast bike rental demand. The data set consists of hourly rental data spanning two years.
It contains the following features: 

• ***Date*** : year-month-day

• ***Rented Bike count*** - Count of bikes rented at each hour

• ***Hour*** - Hour of the day

• ***Temperature***-Temperature in Celsius

• ***Humidity***- %

• ***Windspeed*** - m/s

• ***Visibility*** - 10m

• ***Dew point temperature*** - Celsius

• ***Solar radiation*** - MJ/m2

• ***Rainfall*** - mm

• ***Snowfall*** - cm

• ***Seasons*** - Winter, Spring, Summer, Autumn

• ***Holiday*** - Holiday/No holiday

• ***Functional Day*** - NoFunc(Non Functional Hours), Fun(Functional hours)
 
## Linear Regression
linear regression model assumes that the relationship between the dependent variable and independent is linear. This relationship is modeled through a disturbance term or error variable ε — an unobserved random variable that adds "noise" to the linear relationship between the dependent variable. Thus the model takes the form
Regression is done on numerical data which is continuous.
Linear regression consist of dependent and independent variables related linear to each other
our basic aim is to create best fit line from the dependent and independent variable between two axis, it is expressed in straight line

![Screenshot (227)](https://user-images.githubusercontent.com/85070726/161062232-c2a2a1cc-3dd6-4aac-988f-f0ff85c588ad.png)

Y=B0+B1X1+B2X2+……..+e

B0 is intercept 
b1, b2... are the parameters
Y is actual value
x1,x2 are independent variables 
e is noise

Best fit line in which error between predicted and actual value is minimum. Residual error = (predicted-actual value)2

Our goal is to locate optimum model complexity, if complexity of model exceeded then overfiting of model occur while complexity falls the underfiting will occur in that case we use regularization L1 and L2 it is used to regularize the size of co efficient.

### Lasso regression (L1 Regularization)
It is a type of linear regression that used for shrinkage and to avoid overfitting in the data. To make the optimal solution we use penalty term in cost function and minimize the cost function from value is lambda * mag(Bij) and make final value become zero.

### Ridge Regression (L2 Regularization)
This method performs L2 regularization. When the issue of least-squares are unbiased, and variances are large, this results in predicted values being far away from the actual values. to make the optimal solution we use penalty term in cost function and minimize the cost function from the value is lambda * (Bij)2 and make final value close to zero and shrink the value.

### Decision tree regression model:
Linear model trees combine linear models and decision trees to create a hybrid model that produces better predictions and leads to better insights than either model alone. A linear model tree is simply a decision tree with linear models at its nodes. This can be seen as a piecewise linear model with knots learned via a decision tree algorithm. LMTs can be used for regression problems (e.g. with linear regression models instead of population means) or classification problems (e.g. with logistic regression instead of population modes).

 
## References - 

https://machinelearningmastery.com/linear-regression-for-machine-learning/

https://towardsdatascience.com/linear-regression-detailed-view-ea73175f6e86

Medium
Linear Regression — Detailed View
Linear regression is used for finding linear relationship between target and one or more predictors. There are two types of linear…

