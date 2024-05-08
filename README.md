# Implementation of Multivariate Linear Regression
## Date:
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1:
import pandas as pd.

### Step 2:
Read the csv file.

### Step3:
Get the value of X and y variables

### Step 4:
Create the linear regression model and fit.

### Step 5:
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

## Program:
```
Developed By: Ramya R
Register Number: 2122232230169
import pandas as pd
from sklearn import linear_model
data=pd.read_csv('car.csv')
x=data[['Weight','Volume']]
y=data['CO2']
regression=linear_model.LinearRegression()
regression.fit(x,y)
print("coefficient:",regression.coef_)
print("Intercept:",regression.intercept_)
predictCO2=regression.predict([[3300,1300]])
print("CO2 requried is",predictCO2)
```
## Output:
![alt text](<Screenshot 2024-05-08 185434.png>)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.