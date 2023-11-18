# Implementation of Multivariate Linear Regression
EX 10 Implementation of Multivariate Linear Regression
Date: 08.11.2023
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import panda
### Step2
Import linear model from sklearn
### Step3
Read the file cars.csv
### Step4
Assign the values for x and y as required
### Step5
Create the linearRegression model and predict the output
Program:
## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:", regr.coef_)
print("Intercept:", regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predictedd co2 for the corresponding weight and volume", predictedCO2)
```
## Output:
![280918170-667d3480-7db8-4ca8-a8f7-78676fefa43d](https://github.com/praveenv23013808/Multivariate-Linear-Regression/assets/145824728/8b344989-6663-4a54-b400-e1fb70363bf2)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
