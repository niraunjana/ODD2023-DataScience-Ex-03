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
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/8bd1ee63-50c2-47fb-86a1-632a6e6df26b)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/c67baf58-945b-4c3a-bb43-6aa24c51743b)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/2b3db5a5-979b-4dba-bdb1-d3df1d88bcba)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/43f67a44-7cf9-4967-95da-d549a9f671d4)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/362d91b5-f474-4e7d-b8c5-f4665c413763)
```

Diabetes.csv
```
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/8c025644-7288-450a-a511-92e90614b19f)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/0f6f752d-6370-4061-adba-572e5649e992)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/0d883b88-bf10-4490-83a2-94a51ca0fcb0)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/8479ad6b-35c2-4b76-b012-ce2c76de33b0)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/6da9c239-c63f-44e3-a129-2602dd82acfe)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/df961b0d-5f7d-4908-8f79-ceb299d1f20a)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/72fac76a-f250-4e4c-839a-af90e22b1865)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/535967de-c1af-446d-a862-c39386f0ccc8)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/65ade28f-b152-419a-9110-c5b8942885c1)
![image](https://github.com/niraunjana/ODD2023-DataScience-Ex-03/assets/119395610/73c98ca2-120c-4293-b591-378d4f5e1b11)

### RESULT
Hence the univariate analysis is performed on the given dataset.
