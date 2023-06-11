# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step 1:
Import pandas as pd

Step 2:
Read the csv file

Step 3:
Get the value of X and Y variables

Step 4:
Create the linear regression model and fit

Step 5:
Predict the CO2 emission of a car where the weight is 2300kg and the volume is 1300cm^3

Step 6:
Print the predicted output


## Program:
```
# Developed by: YUVARAJ B
# Reg.No: 212222230182

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("carsemission.csv)
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x.values,y)
print('Coefficients:',regr.coef_)
print('Intercept',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)

```
## Output:

### Insert your output
![244852546-6447f18e-9004-4d42-b7cf-de4af01f0f35](https://github.com/Yuva2005raj/Multivariate-Linear-Regression/assets/118343998/7ec55ff7-3a16-4443-b9bb-8fba531a7a55)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
