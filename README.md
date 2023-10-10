# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1)Import the required packages.

2)Read the data set.

3)Apply label encoder to the non-numerical column inoreder to convert into numerical values.

4)Determine training and test data set.

5)Apply decision tree Classifier and get the values of accuracy and data prediction.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Praveen D
RegisterNumber: 212222240076
import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()

data.info()

data.isnull().sum()

data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()

x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()

y=data["left"]

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)

from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)

y_pred=dt.predict(x_test)

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy

dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:
![image](https://github.com/praveenmax55/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/113497509/0bb8d1c6-4210-4e00-a9e6-c7b227eff7cf)
![image](https://github.com/praveenmax55/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/113497509/649e2a33-0482-46c6-8684-cbe8322faa26)
![image](https://github.com/praveenmax55/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/113497509/55a5bb36-5bbd-4141-8dd4-b24fb6dcf1ac)
![image](https://github.com/praveenmax55/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/113497509/e5057826-1095-4f7a-b0a7-1308c12f9c60)
![image](https://github.com/praveenmax55/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/113497509/95c07948-c295-482e-9b47-e8b4c8f1270c)
![image](https://github.com/praveenmax55/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/113497509/4dd99da6-74ed-4cbb-896b-1ee1f58329b2)
![image](https://github.com/praveenmax55/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/113497509/2162bca3-1052-47f7-9bd3-8ceb092dbfac)
![image](https://github.com/praveenmax55/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/113497509/18ef33f5-3e42-4894-8932-70b8c9192f56)




## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
