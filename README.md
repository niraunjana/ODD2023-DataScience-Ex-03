# ODD2023-DataScience-Ex-03
### Aim:
To read the given data and perform the univariate analysis with different types of plots.

### Eplanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

### Algorithm:
Step 1: Read the given data.

Step 2: Get the information about the data.

Step 3: Remove the null values from the data.

Step 4: Mention the datatypes from the data.

Step 5: Count the values from the data.

### Program:
```
Developed By  : Niraunjana Gayathri G R
Reg No.       : 212222230096
```
```
Superstore.csv
```
```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('SuperStore.csv')
print(df)
df.head()
df.info()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
df.describe()
```
```
Diabetes.csv
```
```
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
df.kurtosis()
```
### OUTPUT
```
Superstore.csv
```
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/f5f03565-7e64-445d-aece-fafd988b162c)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/62763bc6-2965-4b74-ada0-c515db417d95)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/ecae53ae-1547-45e8-8eab-3df4e139e2cd)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/bdca6dd8-39cd-4092-9b09-8fc496c558cb)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/57baca18-7056-4ee2-ab79-0d5130974dd5)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/7e0fedd4-7016-4749-8f39-57a4d51265ab)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/0c5ce859-3868-4b45-9af7-538d009df229)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/215b8cd1-bbe9-4095-8aec-1f55124d5814)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/88032349-076a-4f94-a900-f1e18aece812)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/1af01ec8-46f8-46cc-8bf8-f16635314e52)

