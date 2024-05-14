# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm
## Step 1:
Get the independent variable X and dependent variable Y.
## Step 2:
Calculate the mean of the X -values and the mean of the Y -values.
## Step 3:
Find the slope m of the line of best fit using the formula.
## Step 4:
Compute the y -intercept of the line by using the formula:   
## Step 5:
Use the slope m and the y -intercept to form the equation of the line.
## Step 6:
Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
# Univariate Linear Regression
# Develpoed by:vidhiya lakshmi S
# Register number: 212223230238

import numpy as np
import matplotlib.pyplot as plt 
x=np.array([0,1,2,3,4,5,6,7,8,9])
y=np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(x,y)
plt.show()
xmean=np.mean(x)
ymean=np.mean(y)
num=0
den=0
for i in range(len(x)):
  num+=(x[i]-xmean)*(y[i]-ymean)
  den+=(x[i]-xmean) **2
m=num/den
b=ymean-m*xmean
print(m,b)
ypred=m*x+b
print(ypred)
plt.scatter(x,y,color="Red")
plt.plot(x,ypred, color="Blue")
plt.show()
```
## Output:


<img width="266" alt="image" src="https://github.com/saravidhya/Univariate-Linear-Regression/assets/87062069/1b73307b-1227-47ad-a062-28c5df9f3f8b">










![Screenshot 2024-01-02 152504](https://github.com/priyadharshini210/Univariate-Linear-Regression/assets/148514638/4cb02ef5-2903-460c-8b91-3a89981b035f)

![Screenshot 2024-01-02 152516](https://github.com/priyadharshini210/Univariate-Linear-Regression/assets/148514638/60e2b93c-2ccd-4f7d-962a-f0221592e6e3)
</br>
</br>
</br>
</br>

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
