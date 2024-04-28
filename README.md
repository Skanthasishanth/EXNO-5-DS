# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:

To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:

Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:

STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

## Line Plot:

```
marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()

student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()
```

![ds5_1](https://github.com/Skanthasishanth/EXNO-5-DS/assets/118298456/d99322f9-8c90-48cd-b944-fed7cc503d15)


## Scatter Plot:

```
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()

x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```

![ds5_2](https://github.com/Skanthasishanth/EXNO-5-DS/assets/118298456/4b865cd5-c14c-4797-accd-7ea83cf97c3d)


## Pie Chart:

```
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()

feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```

![ds5_3](https://github.com/Skanthasishanth/EXNO-5-DS/assets/118298456/3ebbaf29-919e-4b85-a311-35a5b7354080)


## Area Chart:

```
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```

![ds5_4](https://github.com/Skanthasishanth/EXNO-5-DS/assets/118298456/3cd03d91-2ad2-41b5-ad8c-85919622c590)


## Bar Chart:

```
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```

![ds5_5](https://github.com/Skanthasishanth/EXNO-5-DS/assets/118298456/400e82d6-684e-4af3-94cf-aae0b5796361)


## Histogram:

```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```

![ds5_6](https://github.com/Skanthasishanth/EXNO-5-DS/assets/118298456/f59587f1-1128-4f0b-b7e9-fefa5ec48de6)


## Box Plot:

```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```

![ds5_7](https://github.com/Skanthasishanth/EXNO-5-DS/assets/118298456/1f44ebb0-8622-4fde-b2fe-ebfefc2edede)


```
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

![ds5_8](https://github.com/Skanthasishanth/EXNO-5-DS/assets/118298456/5e0ad61c-77cc-4a96-949f-1051b0aad855)


# Result:

Thus, all the data visualization techniques of matplotlib has been implemented.
