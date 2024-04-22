# Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student

## AIM:
To write a program to implement the the Logistic Regression Model to Predict the Placement Status of Student.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas for data manipulation and sklearn for machine learning operations.
2. Load data from a CSV file using pandas, then preprocess it by removing unnecessary columns and handling missing values if any. 
3. Divide the preprocessed data into training and testing sets.
4. Train a machine learning model, such as logistic regression (lr), on the training data.

## Program:
```
/*
Program to implement the the Logistic Regression Model to Predict the Placement Status of Student.
Developed by: NITHIYANANDAN N
RegisterNumber: 212222230099
*/

import pandas as pd
data = pd.read_csv("/content/Placement_Data.csv")
data.head()
data1=data.copy()
data1=data1.drop(["sl_no","salary"],axis=1)
data1.head()
data1.isnull().sum()
data1.duplicated().sum()
x=data1.iloc[:,:-1]
x
y=data1["status"]
y
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.metrics import accuracy_score
accuracy = accuracy_score(y_test,y_pred)
accuracy
from sklearn.metrics import confusion_matrix
confusion = (y_test,y_pred)
confusion
from sklearn.metrics import classification_report
classification_report1 = classification_report(y_test,y_pred)
print(classification_report1)
lr.predict([[1,80,1,90,1,1,90,1,0,85,1,85]])
```


## Output:
![image](https://github.com/NITHIYANANDAN278/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121784636/a11da705-31bb-4fe5-9521-2fa9c1c376c9)
![image](https://github.com/NITHIYANANDAN278/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121784636/9d9da3a8-ac86-4813-8cec-3099e93592d6)
![image](https://github.com/NITHIYANANDAN278/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121784636/56b0a83b-1896-4dec-9b7c-5ff0836f6ad2)
![image](https://github.com/NITHIYANANDAN278/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121784636/201b5252-05e4-4569-a344-8d8b94a57022)
![image](https://github.com/NITHIYANANDAN278/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121784636/f8917b1b-cd5b-4df2-85bd-c9994a51bc36)
![image](https://github.com/NITHIYANANDAN278/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121784636/fb3dfacc-8ff9-4fda-a48d-0e827ac13f22)
![image](https://github.com/NITHIYANANDAN278/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121784636/923d3f96-d18f-4ab4-b60d-65c4aedfdbdf)
![image](https://github.com/NITHIYANANDAN278/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121784636/6bebbae8-b9d8-48da-9090-cf0936e4989e)
![image](https://github.com/NITHIYANANDAN278/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121784636/5ff3a7c0-76c5-49cf-a45c-25656c5c9706)
![image](https://github.com/NITHIYANANDAN278/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/121784636/0ecf54d6-67ef-47fc-83e4-c6a7d60e8f3f)



## Result:
Thus the program to implement the the Logistic Regression Model to Predict the Placement Status of Student is written and verified using python programming.
