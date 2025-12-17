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
#Developed by: Sivasakthi S
#Register Number: 25017123

import numpy as np
import matplotlib.pyplot as plt
x=np.array([0,1,2,3,4,5,6,7,8,9])
y=np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(x,y)
plt.show()
x_mean=np.mean(x)
y_mean=np.mean(y)
num=0
den=0
for i in range(len(x)):
    num+=(x[i]-x_mean)*(y[i]-y_mean)
    den+=(x[i]-x_mean)**2
m=num/den
c=y_mean-m*x_mean
print(m, c)




```
## Output
<img width="508" height="358" alt="Screenshot 2025-12-17 172419" src="https://github.com/user-attachments/assets/29ff1b02-5bcd-41ca-8b50-ef9ed5a9ab78" />
<img width="711" height="574" alt="Screenshot 2025-12-17 172430" src="https://github.com/user-attachments/assets/0126e15c-8158-4242-a02c-3e1cf764ba01" />


## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
