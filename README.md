# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1<br>Import Pandas library.
### Step2<br>Import Linear_model from sklearn.
### Step3<br>Read the csv file using pandas library.
### Step4<br>Enter the parameters of the linear function.
### Step5<br>Print the parameters of the linear function.

## Program:
```
DEVELOPED BY : SAMEER SHARIFF M
REGISTER NUMBER : 212224220085
```

```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("/content/car (1).csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```
## Output:
<img width="1437" height="541" alt="image" src="https://github.com/user-attachments/assets/0525c12b-fcb0-4e8b-b0d8-49981e2b092f" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
