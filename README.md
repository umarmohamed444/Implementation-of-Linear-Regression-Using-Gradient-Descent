# Implementation-of-Linear-Regression-Using-Gradient-Descent

## AIM:
To write a program to implement the linear regression using gradient descent.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
~~~
1.Import the required packages.
2.Declare the default values.
3.Predict the y value.
4.Calculate the meansquare error.
5.Plot the graph using the matplotlib.
6.End the program
~~~
 
 

## Program:
```
/*
Program to implement the linear regression using gradient descent.
~~~
Developed by:Umar Mohamed E 
RegisterNumber:212220040173
~~~

import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
data=pd.read_csv("student_scores.csv")
data.head()
data.isnull().sum()
X=data.Hours
X.head()
Y=data.Scores
Y.head()
X_mean=np.mean(X)
Y_mean=np.mean(Y)
n=len(X)
num=0
den=0
Loss=[]
for i in range(len(X)):
    MSE=(1/n)*((Y_mean-Y[i])**2)
    num+=(X[i]-X_mean)*(Y[i]-Y_mean)
    den+=(X[i]-X_mean)**2
    Loss.append(MSE)
m=num/den
c=Y_mean-(m*X_mean)
print (m, c)
Y_pred=(m*X)+c
print (Y_pred)
plt.scatter(X,Y,color='pink')
plt.plot(X,Y_pred,color='blue')
plt.show()

*/
```

## Output:
![Github Logo](umar2.png)


## Result:
Thus the program to implement the linear regression using gradient descent is written and verified using python programming.
