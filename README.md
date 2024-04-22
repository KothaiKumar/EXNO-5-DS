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
```python
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.plot(x_values,y_values)
plt.show()
```
![image](https://github.com/KothaiKumar/EXNO-5-DS/assets/121215739/35c07847-7ce9-40b4-8dc1-b50cedbed213)
```python
import matplotlib.pyplot as plt
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel("y-axis")
plt.title('My first grpah!')
plt.show()
```
![image](https://github.com/KothaiKumar/EXNO-5-DS/assets/121215739/3ce0ecca-0382-4eb7-9622-d9884e7c05ac)
```python
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line 1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line 2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("two lines on same grapg!")
plt.legend()
plt.show()
```
![image](https://github.com/KothaiKumar/EXNO-5-DS/assets/121215739/01a8e899-ec21-4e20-8b74-80efbea4d0f8)
```python
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
```
![image](https://github.com/KothaiKumar/EXNO-5-DS/assets/121215739/d7bf8ab8-eff5-4161-bfbf-f0436c5912e0)
```python
plt.stackplot(x,y1,y2,y3,labels=['line1','line2','line3'])
plt.legend(loc='upper left')
plt.title('stacked line chart')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
![image](https://github.com/KothaiKumar/EXNO-5-DS/assets/121215739/7f5633c7-e1fc-447f-95de-f9ab9d140648)
```python
import numpy as np
import matplotlib.pyplot as plt
values=[5,6,3,7,2]
names=["A","B","C","D","E"]
plt.bar(names,values,color='green')
plt.show()
```
![image](https://github.com/KothaiKumar/EXNO-5-DS/assets/121215739/3b1b8ad4-983d-40fc-a0df-a3c9767f026e)
```python
import matplotlib.pyplot as plt
import numpy as np

ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range = (0, 100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no of people')
plt.title('histogram')
plt.show()
```
![image](https://github.com/KothaiKumar/EXNO-5-DS/assets/121215739/d0382bcc-88f8-4904-af78-823022fe1496)
```python
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/KothaiKumar/EXNO-5-DS/assets/121215739/6495c841-692b-4dda-873b-74ca91f16039)
```python
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel("data")
ax.set_ylabel("values")
ax.set_title("box plot")
```
![image](https://github.com/KothaiKumar/EXNO-5-DS/assets/121215739/1adb8d5e-ee48-4c8c-a808-a798f784f2ca)
```python
import matplotlib.pyplot as plt
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels = slices,colors=colors,startangle=90,shadow = True,explode = (0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
![image](https://github.com/KothaiKumar/EXNO-5-DS/assets/121215739/cb715da6-d2ca-45d0-901d-dbe3ad2c74b6)

# Result:
Thus, Data Visualization using matplot python library is implemented successfully.
