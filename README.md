# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```

#Program to find Univariate Linear Regression
#Developed by:KEERTHIKA M P
#Register Number:212223240071
import numpy as np
import matplotlib.pyplot as plt
y=np.array([1,2,3,4,5])
x=np.array([0,1,3,5,7])
x_mean=np.mean(x)
y_mean=np.mean(y)
num=0
denom=0
for i in range(len(x)):
  num+=(x[i]-x_mean)*(y[i]-y_mean)
  denom+=(x[i]-x_mean)**2
m=num/denom
b=y_mean-m*x_mean
print(m,b)
y_pred=m*x+b
print
plt.scatter(x,y)
plt.plot(x,y_pred,color='red')
plt.show()




```
## Output
![image](https://github.com/Keerthika23013559/Univariate-Linear-Regression/assets/162658262/9c1221ba-619a-491c-93b6-1a8a7ec61ded)


## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
