## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step1

Import panda as pd

Step2

Import linear model from sk learn

Step3

Read the csv file

Step4

Find the multivariate regression

Step5

Display the output

## Program:
```
import pandas as pd 
from sklearn import linear_model 
df=pd.read_csv("/content/car (1).csv") 
x=df[['Weight', 'Volume']] 
y=df['CO2'] 
regr=linear_model.LinearRegression() 
regr.fit(x,y)  
print('Coefficients:',regr.coef_) 
print ('Intercept:', regr.intercept_) 
predictedCO2=regr.predict([[3300,1300]]) 
print("predicted co2 for the correspin weight and vol, ",predictedCO2)



```
## Output:
![Screenshot 2025-05-02 133101](https://github.com/user-attachments/assets/ff7f1cee-b49f-4e87-8a3d-ae4ecb50836d)



### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
