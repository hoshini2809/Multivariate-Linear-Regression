# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd.

### Step2
Read the csv file.

### Step3
Read the csv file.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

## Program:
Developed by: Hoshini S
RegisterNumber: 2305003006
import pandas as pd
  from sklearn import linear_model
  df=pd.read_csv("car.csv")
  x=df[['Weight','Volume']]
  y=df['CO2']
  regr=linear_model.LinearRegression()
  regr.fit(x,y)
  print("Coefficient:",regr.coef_)
  print("Intercept:",regr.intercept_)
  predictedCO2=regr.predict([[3300,1300]])
  print("Predicted CO2 for the corresponding weight and volume",predictedCO2)
  
## Output:

![Screenshot 2024-05-24 204952](https://github.com/hoshini2809/Multivariate-Linear-Regression/assets/170595101/b2c9ce40-9813-4b3c-a30b-ebd415fb6ac2)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
