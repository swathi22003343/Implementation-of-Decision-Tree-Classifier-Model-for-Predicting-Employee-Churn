# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## Aim:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm:

1. Import the required libraries.
2. Upload and read the dataset.
3. Check for any null values using the isnull() function.
4. From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.
5. Find the accuracy of the model and predict the required values by importing the required module from sklearn.

## Program:
```
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: SWATHI D
RegisterNumber: 212222230154

import pandas as pd
data=pd.read_csv("/content/Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x.head()
y = data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt = DecisionTreeClassifier(criterion = "entropy")
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
from sklearn import metrics
accuracy = metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
```

## Output:

### data.head():
![ml exp-6-1](https://github.com/Gopika-9266/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/122762773/9bd394fc-03c0-4558-939e-b4803aa33752)

### data.info():
![ml exp6-2](https://github.com/Gopika-9266/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/122762773/61749dd9-f56b-4d59-9d8e-408e8762f851)

### data.isnull().sum():
![ml exp6-3](https://github.com/Gopika-9266/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/122762773/26416138-1cf6-435e-b391-0721659fde12)

### data value count:
![ml exp6-4](https://github.com/Gopika-9266/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/122762773/f7c06b25-2c79-40ee-9715-809f01219817)

### data head() for salary:
![ml exp6-5](https://github.com/Gopika-9266/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/122762773/1d604b98-e0b7-4330-be9b-9c653403085e)

### x.head():
![ml exp6-6](https://github.com/Gopika-9266/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/122762773/841a4843-43b9-48c1-967d-2480f67700af)


### Accuracy value:
![ml exp6-7](https://github.com/Gopika-9266/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/122762773/4553a8c9-fcfc-4f0c-b8ff-0f64c43a92d7)

### Data prediction:
![ml exp6-8](https://github.com/Gopika-9266/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/122762773/337512f3-74c7-457d-a184-76498b2ffd63)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
