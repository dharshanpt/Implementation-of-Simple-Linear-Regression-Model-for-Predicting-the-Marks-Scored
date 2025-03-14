## Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored:

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm:
```

step 1. Start the program.
step 2. To implement the linear regression using the standard libraries in the python.
step 3. Use slicing function() for the x,y values.
step 4. Using sklearn library import training , testing and linear regression modules.
step 5. Predict the value for the y.
step 6. Using matplotlib library plot the graphs.
step 7. Use xlabel for hours and ylabel for scores.
step 8. End the porgram.
```
## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: DHARSHAN PT
RegisterNumber: 212223230046

import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
df=pd.read_csv('/content/student_scores - student_scores.csv')
df.head()
X=df.iloc[:,:-1].values
X
y=df.iloc[:,1].values
y
from sklearn.model_selection import train_test_split
X_train,X_test,y_train,y_test=train_test_split(X,y,test_size=1/3,random_state=0)
from sklearn.linear_model import LinearRegression
regressor=LinearRegression()
regressor.fit(X_train,y_train)
y_pred=regressor.predict(X_test)
y_pred
y_test
plt.scatter(X_train,y_train,color='violet')
plt.plot(X_train,regressor.predict(X_train),color="black")
plt.title("h vs s (Training Set)")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()
plt.scatter(X_test,y_test,color='purple')
plt.plot(X_test,regressor.predict(X_test),color="black")
plt.title("h vs s (Testing Set)")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()

*/
```

## Output:
![Screenshot 2024-08-28 080724](https://github.com/user-attachments/assets/21d1728e-4b3e-4250-9a48-8ebc7df4b7d7)

![Screenshot 2024-08-28 080739](https://github.com/user-attachments/assets/2d68db98-d500-41ca-918e-daf1570507ad)





## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
