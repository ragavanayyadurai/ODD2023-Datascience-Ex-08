# Ex-08 Data Visualization
# Aim:
To Perform Data Visualization on a complex dataset and save the data to a file.

# Explanation:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:

## STEP 1:
Read the given Data

## STEP 2:
Clean the Data Set using Data Cleaning Process

## STEP 3:
Apply Feature generation and selection techniques to all the features of the data set

## STEP 4:
Apply data visualization techniques to identify the patterns of the data.

# Code and Output:

Name: Ragavendran A

Reg no: 212222230114

```python
  import matplotlib.pyplot as plt

  x_values=[0,1,2,3,4,5]
  y_values=[0,1,4,9,16,25]

  plt.plot(x_values,y_values)
```

<img width="211" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/62066b98-3238-4394-bedc-331a296ade4e">

```python
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-values')
plt.ylabel('y-values')
plt.title('My first graph')
```

<img width="219" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/f96c45d7-4b6d-4d70-ac89-65b1bad32285">

```python
x1=[1,2,3]
y1=[2,4,1]
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x1,y1,label='line 1')
plt.plot(x2,y2,label='line 2')
plt.xlabel('x-values')
plt.ylabel('y-values')
plt.title('Two lines on same graph')
```

<img width="220" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/d33b3bc0-651a-4acb-a65e-2b4c47c3358c">

```python
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]

plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-values')
plt.ylabel('y-values')
plt.title('some cool customizations')
```

<img width="218" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/9723d83a-ce4a-4f8f-b0e2-735459f3fc03">

```python
yield_apples=[0.8,0.91,0.919,0.926,0.929,0.93]
plt.plot(yield_apples)
```

<img width="215" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/56087dcd-bdfe-4c4e-a842-1c2a4f63b609">

```python
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```

<img width="218" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/9b023cd4-158e-4b5d-ad23-3631b5b512f5">

```python
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='yellow')
plt.plot(x,y1,color='black')
plt.plot(x,y2,color='white')
plt.legend(['y1','y2'])
```

<img width="216" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/3b558436-58bd-4a93-8b3c-1998c96ea28b">

```python
import seaborn as sns
import matplotlib.pyplot as plt

x=[1,2,3,4,5]
y=[3,6,2,7,1]

sns.lineplot(x=x,y=y)
```

<img width="208" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/1b053752-e82e-43c0-bdd3-262b287a150a">

```python
x=[1,2,3,4,5]
y1=[3,5,2,6,1]
y2=[1,6,4,3,8]
y3=[5,2,7,1,4]

sns.lineplot(x=x,y=y1)
sns.lineplot(x=x,y=y2)
sns.lineplot(x=x,y=y3)
plt.title("Multi-Line Plot")
plt.xlabel("X Label")
plt.ylabel("Y Label")
```

<img width="219" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/1f86e82c-ee41-4405-a6af-fc92062c0584">

```python
import matplotlib.pyplot as plt
values=[5,6,3,7,2]
names=["A","B","C","D","E"]
plt.bar(names,values,color="green")
plt.show()
```

<img width="205" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/e8ddac2b-2a32-4ac8-824e-e67c59f3cc30">

```python
plt.barh(names,values,color="black")
plt.show()
```

<img width="206" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/8fad88c2-9c56-44e5-a5b6-a54559e006de">

```python
height=[10,24,36,40,5]
names=["one","two","three","four","five"]
c1=["red","green"]
c2=["b","g"]
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.title("My Bar chart!!!!!!!!!!!!")
```

<img width="217" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/3e67e6e4-ab29-45ab-9310-a257ddb0a61f">

```python
import seaborn as sns
import matplotlib.pyplot as plt
tips= sns.load_dataset("tips")
avg_total_bill = tips.groupby("day")['total_bill'].mean()
avg_tip =tips.groupby('day')['tip'].mean()
plt.figure(figsize=(8, 6))
p1 = plt.bar(avg_total_bill.index, avg_total_bill, label='Total Bill')
p2 = plt.bar(avg_tip.index, avg_tip, bottom=avg_total_bill, label='Tip')
plt.xlabel('Day of the Week')
plt.ylabel('Amount')
plt.title("Average total bil and tip by day")
plt.legend()
```

<img width="265" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/b5e6b932-34c9-44a4-a5ad-6d50b63c192e">

```python
import seaborn as sns
dt=sns.load_dataset("tips")
sns.barplot(x="day",y="total_bill",hue="sex",data=dt,palette="Set1")
plt.xlabel('Day of the Week')
plt.ylabel('Total bill')
plt.title("Total bill by day and gender")
```

<img width="216" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/4b127999-c0cd-45ca-8604-1e224b0f3c31">

```python
import pandas as pd
tit=pd.read_csv("/content/titanic_dataset.csv")

plt.figure(figsize=(8,5))
sns.barplot(x="Embarked",y="Fare",data=tit,palette="rainbow")
plt.title("Fare of passengers by embarked town")
```

<img width="264" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/d51d08a9-529b-4c17-aae2-72ef2d9c8be7">

```python
import matplotlib.pyplot as plt
x_values = [0,1,2,3,4,5]
y_values = [0,1,4,9,16,25]
plt.scatter (x_values, y_values, s=30, color="blue")
plt.show()
```

<img width="205" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/5e48231f-73b5-4503-bf1f-2943cdd73aee">

```python
x = [1,2,3,4,5,6,7,8,9,10]
y = [2,4,5,7,6,8,9,11,12,12]
plt.scatter(x,y,label = "stars",color='green',marker='*',s=30)
plt.title("scatter plot")
plt.legend()
```

<img width="209" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/8d16332a-8a57-4efc-92e5-286e6c989318">

```python
import seaborn as sns
tips = sns.load_dataset('tips')
sns.scatterplot(x= 'total_bill', y='tip', hue='sex',data=tips)
plt.xlabel('Total Bill')
plt.ylabel('Tip Amount')
plt.title('Scatter Plot of Total Bill vs. Tip Amount')
```

<img width="217" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/2c9ff2c3-291a-4768-80cf-4bc2bf60308b">

```python
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color="green",histtype="bar",rwidth=0.8)
plt.xlabel("age")
plt.ylabel("No.of.People")
plt.title("My Histogram")
```

<img width="215" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/12058377-ad6b-49ff-a586-5ec37b309b77">

```python
x=[2,1,6,2,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color="black",alpha=0.5)
```

<img width="224" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/1146410a-68bf-42e3-a6f3-7ca55f0aad88">

```python
import seaborn as sns
import numpy as np
import pandas as pd

np.random.seed(1)
num_var=np.random.randn(1000)
num_var=pd.Series(num_var,name="Numerical Variable")
num_var
```

<img width="168" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/f3630c83-45e0-468c-b67a-0efa5f69e3f3">

```python
sns.histplot(data=num_var,kde=True)
```

<img width="221" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/4252a824-d89f-4b00-8065-0ca6a8d03294">

```python
import pandas as pd
import seaborn as sns
df=pd.read_csv("/content/titanic_dataset.csv")

sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
```

<img width="222" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/47a707b0-d38d-4c2f-a6cb-ab037fe0b48d">

```python
import matplotlib.pyplot as plt
import numpy as np

np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```

<img width="216" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/3be1db4d-fe21-43ff-9750-916b4d5cf173">

```python
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel("Data")
ax.set_ylabel("Values")
ax.set_title("Boxplot")
```

<img width="218" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/4acb2dff-c4f3-4fcd-b69f-7359e67aa37b">

```python
import seaborn as sns
import pandas as pd
tips = sns.load_dataset('tips')
sns.boxplot(x=tips["day"], y=tips["total_bill"], hue=tips["smoker"], data = tips)
```

<img width="218" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/6e6f076f-2a51-4939-b5cd-0e9f6e274e47">

```python
sns.boxplot(x="day", y="total_bill", hue="smoker", data=tips, linewidth=2, width=0.6,boxprops={"facecolor": "lightblue", "edgecolor": "darkblue"},
whiskerprops={"color": "black", "linestyle":"--", "linewidth": 1.5 },capprops={"color": "black", "linestyle": "--", "linewidth":1.5})
```

<img width="217" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/7d1b8007-9878-4b77-ac2f-ebb5765d81d1">

```python
sns.boxplot(x='day',y='total_bill',data= tips)
plt.title("Age by Passenger Class, Titanic")
```

<img width="212" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/20acac01-c089-4d1d-9b10-d232b42a5ea7">

```python
sns.violinplot (x="day", y="total_bill", hue="smoker", data= tips, linewidth=2, width=0.6,)
```

<img width="217" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/5f38b103-8668-4fc2-b58e-4255b8f459d8">

```python
data = np.random.randint(low = 1, high = 100, size = (10,10))
print("The data to be plotted: \n")
print (data)
```

<img width="106" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/fc4c5b41-b295-4cab-835c-fdb55fa8986d">

```python
hm=sns.heatmap(data=data)
```

<img width="194" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/c41b68ae-65a1-4645-80a8-2f99f5a5c792">

```python
import pandas as pd
import seaborn as sns
df=pd.read_csv("/content/titanic_dataset.csv")

import matplotlib.pyplot as plt
ages= [2,5, 70, 40, 30, 45, 50,45, 43, 40,44, 60, 7,13, 57, 18, 90, 77,32, 21, 20, 40]
range = (0, 100)
bins = 10
sns.histplot(data=df,x="Pclass",hue="Survived")
plt. xlabel ('age')
plt.ylabel ('No. of people')
plt. title ('My histogram')
plt.show()
```

<img width="215" alt="image" src="https://github.com/TejaswiniGugananthan/ODD2023-Datascience-Ex-08/assets/121222763/0eaeb615-8428-431d-b371-d4db554fbde6">


# Result:
Hence the data visualization method for the given dataset applied successfully.
