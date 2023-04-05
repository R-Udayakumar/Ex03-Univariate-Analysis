# Ex03-Univariate-Analysis

## Aim

To read the given data and perform the univariate analysis with different types of plots.

## Explanation :

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## Algorithm

### STEP 1
Read the given data.

### STEP 2
Get the info about the data.

### STEP 3
Discribe the readed data using describe method.

### STEP 4
Mention the datatypes from the data.

### STEP 5
Count the values from the data.

### STEP 6
Finally Analyze the data using different types of plot method.

## Program
```python
# Developed By Udayakumar R
# Reference No: 22008609

# [1]
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv('SuperStore.csv')
print(df)
df.head()
df.info()
df.dtypes
df['Sales'].value_counts()
df.describe()
sns.boxplot(x="Row ID",data=df)
sns.countplot(x="Order ID",data=df)
sns.distplot(df["Sales"])
sns.histplot(x="Region",data=df)

# [2]
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv('diabetes.csv')
df.head()
df.info()
df.dtypes
df['BMI'].value_counts()
df.describe()
sns.boxplot(x="Age",data=df)
sns.countplot(x="Age",data=df)
sns.distplot(df["Age"])
sns.histplot(x="Age",data=df)
df.skew()
sns.histplot(x="Insulin",data=df)
sns.displot(x="BloodPressure",data=df)
df.kurtosis()
sns.boxplot(x="Insulin",data=df)
sns.boxplot(x="SkinThickness",data=df)

```
## OUTPUT
```
 [1]
```
#### HEAD DATA :
![image](https://user-images.githubusercontent.com/118708024/230036526-549ba838-506f-455f-b2df-5fb41346181b.png)

#### INFO DATA :
![image](https://user-images.githubusercontent.com/118708024/230035997-e90081a4-c592-4d81-92f8-c9e0fe5f2236.png)

#### DATA DESCRIBE :
![image](https://user-images.githubusercontent.com/118708024/230037430-41a3ee10-6331-4ecd-8829-803d42694e18.png)

#### DATA TYPES :
![image](https://user-images.githubusercontent.com/118708024/230038269-dff68887-dd73-4a6e-9b87-e81daa792def.png)

#### VALUE COUNT :
![image](https://user-images.githubusercontent.com/118708024/230036760-644f8704-79d8-4b72-996d-d73e40f787cf.png)

#### BOXPLOT :
![image](https://user-images.githubusercontent.com/118708024/230038000-e013784d-d8ff-48cd-924b-3924ccf15655.png)

#### COUNTPLOT :
![image](https://user-images.githubusercontent.com/118708024/230037912-715b768d-a631-4cc8-b5d4-896bb74d2500.png)

#### HISTOGRAM PLOT :
![image](https://user-images.githubusercontent.com/118708024/230037803-9203e4a5-2615-4853-b830-73d6f33327bd.png)

#### DISTRIBUTION PLOT :
![image](https://user-images.githubusercontent.com/118708024/230037666-3682fc72-57ce-4ad4-bad6-cc85686e41f8.png)
```
[2]
```
#### HEAD DATA :
![image](https://user-images.githubusercontent.com/118708024/230038777-90306705-8f8b-40a9-8e21-1c990ef3e3ff.png)
#### INFO DATA :
![image](https://user-images.githubusercontent.com/118708024/230038592-80dab84f-a210-4d52-bb0b-4dcb2f86f0f5.png)
### DATA TYPES :
![image](https://user-images.githubusercontent.com/118708024/230039171-78bdab37-4de0-4571-9570-47d18b1e0b5f.png)
### DATA DESCRIBE:
![image](https://user-images.githubusercontent.com/118708024/230039375-66e6a650-0ddb-4212-ac59-6d83c84f814e.png)
### VALUE COUNTS :
![image](https://user-images.githubusercontent.com/118708024/230039647-d2c48cc9-4e1a-4504-a143-d57a27a5d71c.png)
### BOX PLOT :

## RESULT
Therefore we have read the given data and performed the univariate analysis with different types of plots.
