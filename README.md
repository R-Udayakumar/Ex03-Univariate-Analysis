# Ex03-Univariate-Analysis

## Aim

To read the given data and perform the univariate analysis with different types of plots.

## Explanation

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## Algorithm

### STEP 1
Read the given data.

### STEP 2
Get the information about the data.

### STEP 3
Remove the null values from the data.

### STEP 4
Mention the datatypes from the data.

### STEP 5
Count the values from the data.

### STEP 6
Do plots like boxplots,countplot,distribution plot,histogram plot.

## Program
```python
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv('SuperStore.csv')
print(df)
df.head()
df.info()
df.describe()
df.dtypes
df.isnull().sum()
df['Postal Code'] = df["Postal Code"].fillna(df['Postal Code'].mode()[0])
df.isnull().sum()
df['Postal Code'].value_counts()
sns.boxplot(x="Postal Code",data=df)
sns.distplot(df["Sales"])
sns.countplot(x="Sales",data=df)
sns.histplot(x="Sales",data=df)
sns.boxplot(x="Sales",data=df)
snb.countplot(x="Product ID",data=df)
sns.countplot(x="Category",data=df)
sns.histplot(x="Product ID",data=df)
sns.displot(x="Postal Code",data=df)
```
## OUTPUT

#### DATA FRAME : 
![image](https://user-images.githubusercontent.com/118708024/229819206-54235db7-8fda-431f-a041-afafb57b4b27.png)

#### HEAD DATA :
![image](https://user-images.githubusercontent.com/118708024/229818621-694f3826-afde-4d60-bd93-7f2e2a7eb3db.png)

#### INFO DATA :
![image](https://user-images.githubusercontent.com/118708024/229819973-25d7fc52-c59f-46b5-99b0-de89596e75d1.png)

#### DATA DESCRIBE :
![image](https://user-images.githubusercontent.com/118708024/229820546-161b91f5-fafe-427f-971d-036fad98e5b1.png)

#### NULL VALUES :
![image](https://user-images.githubusercontent.com/118708024/229820846-f22f1953-13ce-4266-b823-30db4ab43ff8.png)

#### DATA TYPES :
![DS6](https://user-images.githubusercontent.com/93427345/191899082-b33f146f-342f-4f3a-91eb-a75f3df20ffc.PNG)

#### VALUE COUNT :
![DS7](https://user-images.githubusercontent.com/93427345/191899148-cd36cef2-1862-47bc-b22d-5b103fceb4cb.PNG)

#### BOXPLOT :
![DS8](https://user-images.githubusercontent.com/93427345/191899185-be661814-d402-4245-ba45-cbe649579323.PNG)

#### COUNTPLOT :
![DS9](https://user-images.githubusercontent.com/93427345/191899219-e401211a-2cfc-4307-94c8-80141da63e6c.PNG)

#### DISTRIBUTION PLOT :
![DS10](https://user-images.githubusercontent.com/93427345/191899278-36e61237-4504-4203-b341-bb5da1c7a3e8.PNG)

#### HISTOGRAM PLOT :
![DS11](https://user-images.githubusercontent.com/93427345/191899301-c3316b5a-2418-44e3-8422-c2e772aca695.PNG)

## RESULT
Thus we have read the given data and performed the univariate analysis with different types of plots.
