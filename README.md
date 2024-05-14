# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Start the program
2. Import pandas
3. Import Decision tree classifier
4. Fit the data in the model
5. Find the accuracy score
6. End the program

## Program:
```
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: MIDHUN S
RegisterNumber:  212223240087
```
```
import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
```
```
x=data[["Position","Level"]]
x.head()
y=data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred) 
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
```

## Output:
#### data.head()
![exp 7 1](https://github.com/23003250/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/139331462/566ce1f5-3c40-401b-b4ec-105a6a986277)

#### data.info()
![exp 7 2](https://github.com/23003250/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/139331462/0388ac9b-6f74-4055-a090-dca2d9c481b3)
<br><br><br><br><br>
#### isnull() and sum()
![exp 7 3](https://github.com/23003250/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/139331462/1ed92366-a8b8-4b6d-b7ce-6468749db08a)

#### data.head() for salary 
![exp 7 4](https://github.com/23003250/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/139331462/6be8745a-1ffe-4589-a073-4a6c7bb7a2cd)

#### MSE value
![exp 7 5](https://github.com/23003250/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/139331462/a6e80f83-0987-44c9-bc5d-ad1d332cf868)

#### r2 value
![exp 7 6](https://github.com/23003250/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/139331462/c36dd21f-a7cb-4091-a8af-0e376ab2931d)

#### data prediction
![exp 7 7](https://github.com/23003250/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/139331462/33e7b744-fa7b-42a7-88e2-c3a2d6f1cc74)

 
## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
