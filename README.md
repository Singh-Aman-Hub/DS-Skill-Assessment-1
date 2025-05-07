```
Developed by: Aman Singh || Register no.: 212224040020
```
```
import pandas as pd
import numpy as np
df= pd.read_csv("/content/SAMPLEIDS.csv")
df.head()

```
<img width="433" alt="Screenshot 2025-05-06 at 7 44 15 PM" src="https://github.com/user-attachments/assets/55e29ddd-49aa-4882-9378-d2ff4253d3d2" />

```
df.isnull()
```
<img width="384" alt="Screenshot 2025-05-06 at 7 44 25 PM" src="https://github.com/user-attachments/assets/1cde06a2-c80f-4a82-bcdf-a4d50c1fa79b" />


```
df.fillna(method='ffill')
```
<img width="485" alt="Screenshot 2025-05-06 at 7 45 12 PM" src="https://github.com/user-attachments/assets/9682384c-f776-4068-8bb2-394c91b34ebd" />

```
df.describe()
```
<img width="430" alt="Screenshot 2025-05-06 at 7 45 30 PM" src="https://github.com/user-attachments/assets/ca7f62af-b65b-4649-87f8-37b3274287e7" />

```
df = pd.DataFrame({'col1':[1,2,3,4],'col2':[444,555,666,444],
			'col3':['abc','def','ghi','xyz']})
df.sort_values(by='col2')

```
<img width="181" alt="Screenshot 2025-05-06 at 7 46 06 PM" src="https://github.com/user-attachments/assets/cf7a9b77-9664-4464-ad09-032179d9e25c" />


```
df = pd.DataFrame(np.random.randn(10,2),
		index=[1,4,6,2,3,5,9,8,0,7],columns = ['col2','col1'])
df


```
<img width="141" alt="Screenshot 2025-05-06 at 7 46 13 PM" src="https://github.com/user-attachments/assets/91414b4e-c307-4f6f-b3ff-771353e8243d" />

```
df1=df.sort_index(ascending=False)
print(df1)
df2=df.sort_index()
print(df2)
```
<img width="203" alt="Screenshot 2025-05-06 at 7 46 36 PM" src="https://github.com/user-attachments/assets/f6cdd997-22d2-4d03-8239-9a6b1ee385ae" />

```
data = {'Company':['GOOG','GOOG','MSFT','MSFT','FB','FB'],
       'Person':['Sam','Charlie','Amy','Vanessa','Carl','Sarah'],
       'Sales':[200,120,340,124,243,350]}
df = pd.DataFrame(data)
df

```
<img width="173" alt="Screenshot 2025-05-06 at 7 47 08 PM" src="https://github.com/user-attachments/assets/d93a9dc3-43fc-4d34-8a10-cc73011c641d" />

```
df.groupby('Company')['Sales'].mean()

```
<img width="138" alt="Screenshot 2025-05-06 at 7 47 19 PM" src="https://github.com/user-attachments/assets/c63a469a-2504-40da-9b4e-3a50c0b5549d" />

```
df.groupby('Company')['Sales'].std()


```
<img width="160" alt="Screenshot 2025-05-06 at 7 47 30 PM" src="https://github.com/user-attachments/assets/2cc35fcc-1802-4d4c-99c7-0f32eadd33f1" />


```
import pandas as pd
data = {
    'Name': ['John', 'Sarah', 'Mike', 'Emily', 'David'],
    'Age': [25, 31, 29, 35, 27],
    'Gender': ['M', 'F', 'M', 'F', 'M'],
    'Salary': [50000, 70000, 60000, 80000, 55000]
}
df = pd.DataFrame(data)
print(df.head(3))

```


<img width="150" alt="Screenshot 2025-05-06 at 7 47 43 PM" src="https://github.com/user-attachments/assets/56b83f89-67fc-410b-8aca-2c923144cd08" />

```
import pandas as pd
data = {
'Name': ['John','Sarah', 'Mike', 'Emily', 'David'],
'Age': [25, 31, 29, 35, 27],
'Gender': ['M', 'F', 'M','F','M'],
'Salary': [50000, 70000, 60000, 80000, 55000]
}
df = pd. DataFrame(data)
print(df.tail(3))
```
<img width="186" alt="Screenshot 2025-05-06 at 7 48 06 PM" src="https://github.com/user-attachments/assets/ee192545-d6a8-425c-b9bb-2932ecd33069" />

```

import pandas as pd;
data = {
    'Name': ['John','Sarah','Mike', 'Emily', 'David'],
    'Age': [25, 31, 29, 35, 27],
    'Gender': ['M','F','M','F','M'],
    'Salary': [50000, 70000, 60000, 80000, 55000]
    }
df = pd.DataFrame(data)
df.info()

```
<img width="162" alt="Screenshot 2025-05-06 at 7 48 28 PM" src="https://github.com/user-attachments/assets/a85e37be-641c-4601-b3c0-4ee9fa9104fa" />

```
data = {
    'Name': ['John','Sarah','Mike', 'Emily', 'David'],
    'Age': [25, 31, 29, 35, 27],
    'Gender': ['M','F','M', 'F','M'],
    'Salary': [50000, 70000, 60000, 80000, 55000]
}
df = pd.DataFrame (data)
print(df.describe())
```
<img width="210" alt="Screenshot 2025-05-06 at 7 48 40 PM" src="https://github.com/user-attachments/assets/5cc85c96-0f0c-4d6a-9454-15faf278db2e" />

```
data = {'name': ['Alice', 'Bob', 'Charlie', 'Dave', 'Emily', 'Frank'],
        'gender' : ['F', 'M', 'M', 'M', 'F', 'M'],
          'age': [25, 35, 40, 28, 30, 45],
        'salary': [50000, 70000, 60000, 80000, 65000, 90000]}
df = pd.DataFrame(data)
grouped = df.groupby('gender')['salary'].mean()
print(grouped)

```
<img width="189" alt="Screenshot 2025-05-06 at 7 48 57 PM" src="https://github.com/user-attachments/assets/f6cc4443-c24c-4276-b584-92d7661c9c67" />


```
data = {'name': ['Alice', 'Bob', 'Charlie', 'Dave', 'Emily', 'Frank'],
      'gender': ['F','M', 'M', 'M', 'F', 'M'],
        'age': [25, 35, 40, 28, 30, 45],
        'salary': [50000, 70000, 60000, 80000, 65000, 900001]}
df = pd.DataFrame(data)
grouped = df.groupby('gender').count()
print (grouped)

```
<img width="182" alt="Screenshot 2025-05-06 at 7 49 09 PM" src="https://github.com/user-attachments/assets/c59cc623-8755-456b-beb2-8fe9de70a6e8" />
```
import pandas as pd
# Create a sample DataFrame with missing values
data = {'Name': ['Alice', 'Bob', 'Charlie', 'Dave', 'Eve'],
'Age': [25, 32, None, 41, 28],
'Salary': [50000, None, 70000, 90000, 60000]}
df = pd.DataFrame (data)
df

```
<img width="215" alt="Screenshot 2025-05-06 at 7 49 29 PM" src="https://github.com/user-attachments/assets/bf43f74d-a236-4419-9fcf-313b3b31f676" />

```
df_cleaned = df.dropna(subset=['Salary'])
print(df_cleaned)

```
<img width="152" alt="Screenshot 2025-05-06 at 7 49 38 PM" src="https://github.com/user-attachments/assets/b5b2e224-eef0-4fef-95fe-2d150593d5a4" />

```
# Remove rows with all missing values
df_cleaned_all = df.dropna(how='all')
print(df_cleaned_all)

```
<img width="161" alt="Screenshot 2025-05-06 at 7 50 10 PM" src="https://github.com/user-attachments/assets/494dd9aa-156f-405f-b5a5-78cdcbf344e7" />
```
df_cleaned_any = df.dropna (how='any')
print(df_cleaned_any)

```
<img width="142" alt="Screenshot 2025-05-06 at 7 50 29 PM" src="https://github.com/user-attachments/assets/a5f8b28e-9c5f-4324-aba1-bcdc921a0c29" />

```
data = {'Name': ['Alice', 'Bob', 'Charlie', 'Dave', 'Dave', 'Eve', 'Bob'],
        'Age': [25, np.nan, 35, 41, np.nan,np.nan, 85],
        'Salary': [50000, np.nan, 70000, np.nan, 60000, np.nan, 70000]}
df = pd.DataFrame(data)
df.duplicated()

```
<img width="81" alt="Screenshot 2025-05-06 at 7 50 47 PM" src="https://github.com/user-attachments/assets/8c3ff3ba-d2dc-4c30-88f6-b812740150d9" />

```
data = {'Name': ['Alice', 'Bob', 'Charlie', 'Dave', 'Eve'],
'Age': [25, np.nan, 35, 41, np.nan],
'Salary': [50000, np.nan, 70000, np.nan, 60000]}
df = pd.DataFrame(data)

df_filled = df.fillna(0)
print(df_filled)

```
<img width="159" alt="Screenshot 2025-05-06 at 7 51 03 PM" src="https://github.com/user-attachments/assets/8cdf82b6-3b14-4ee4-b1ad-7977a652b5d6" />

```
data = {'name': ['Alice', 'Bob', 'Charlie', 'Dave'],
        'age': [25, 32, 18, 471],
        'gender': ['F',' M',' M','M'],
        'height':[1.62, 1.78, 1.65, 1.831]}
df = pd. DataFrame (data)
df_filtered = df[(df ['gender']== 'M') & (df['height'] >1.7)]
df_filtered
```
<img width="200" alt="Screenshot 2025-05-06 at 7 51 15 PM" src="https://github.com/user-attachments/assets/51f1fc07-78d1-4e57-8009-61169cd107f5" />
