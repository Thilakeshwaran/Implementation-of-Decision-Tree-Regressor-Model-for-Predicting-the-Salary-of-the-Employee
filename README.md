# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm:
1. Import the standard libraries.
2. Upload the dataset and check for any null values using .isnull() function.
3. Import LabelEncoder and encode the dataset.
4. Import DecisionTreeRegressor from sklearn and apply the model on the dataset.
4. Predict the values of arrays.
5. Import metrics from sklearn and calculate the MSE and R2 of the model on the dataset.
6. Predict the values of array.
7. Apply to new unknown values.
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: THILAKESWARAN KP
RegisterNumber: 212223230232

import pandas as pd
data=pd.read_csv("Salary.csv")

data.head()

data.info()

data.isnull().sum()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()

x=data[["Position", "Level"]]
y=data["Salary"]

from sklearn.model_selection import train_test_split
x_train,x_test,y_train, y_test=train_test_split(x, y, test_size=0.2, random_state=2)

from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train, y_train)
y_pred=dt.predict(x_test)

from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse

r2=metrics.r2_score(y_test,y_pred)
r2

dt.predict([[5,6]])
*/
```

## Output:
![Screenshot 2024-10-12 133044](https://github.com/user-attachments/assets/04953e91-39d8-44be-8d79-81e8a0e083f0)

![Screenshot 2024-10-12 133050](https://github.com/user-attachments/assets/549f0355-f429-4b17-a5ad-f0955a570874)

![Screenshot 2024-10-12 133111](https://github.com/user-attachments/assets/666b4b0b-cbe7-466f-9700-580108b7e7ef)

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
