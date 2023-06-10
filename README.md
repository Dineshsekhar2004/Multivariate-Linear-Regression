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
Read the CSV file.

### Step3
Get the value of x and y variables.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 2300Kg, and the volume is 1300cm3.

### Step6
Print the predicted output.

## Program:
```
Developed by: Dinesh.S
Reg No: 212222230033
```


```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Interact:",regr.intercept_)
print("Amount:",regr.predict([[3000,1300]]))






```
## Output:
![image](https://github.com/Dineshsekhar2004/Multivariate-Linear-Regression/assets/119405916/36965c03-2359-4198-915b-962065131729)




## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
