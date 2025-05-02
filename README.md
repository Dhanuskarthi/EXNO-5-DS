# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY
```
Name-Dhanus karthi s
Reg no-24005701
```
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
x1 = [1,2,3]
y1 = [2,4,1]
x2 = [1,2,3]
y2 = [4,1,3]
plt.plot(x1,y1,label='line1')
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```
![download](https://github.com/user-attachments/assets/6302b079-ccdf-4e84-a39d-1b5846d9712e)
```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
```
![download](https://github.com/user-attachments/assets/4728d29e-892f-48f5-85ed-e80a732c30c2)
```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![download](https://github.com/user-attachments/assets/c9ecfa4b-92ee-42fb-aa70-4f7c7b2221e7)
```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```
![download](https://github.com/user-attachments/assets/a6cdd439-3483-435e-9929-31093a4f1c2c)
```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);
```
![download](https://github.com/user-attachments/assets/7a22810f-8f10-485d-a041-8bfdacc311a5)
```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```
![download](https://github.com/user-attachments/assets/e470061a-7410-475c-8be7-8c33092b377b)
![image](https://github.com/user-attachments/assets/aa1533c1-7ef7-4f07-8596-ddd82293244a)
```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![download](https://github.com/user-attachments/assets/1a029b0f-258b-4172-abe6-889439aa3575)
![image](https://github.com/user-attachments/assets/ae9fa82b-953f-4c71-9af1-77c0accb4c24)
```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.legend(['y-values']);
```
![download](https://github.com/user-attachments/assets/ef333004-ef80-4d70-ac09-1180b7853508)
```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
![download](https://github.com/user-attachments/assets/be977971-32fc-4c4b-ac95-b0f1a8885123)
```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```
![download](https://github.com/user-attachments/assets/f4ef72fa-730a-4310-8465-cde7985987a7)
```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![download](https://github.com/user-attachments/assets/b7f694df-0224-4170-b721-9ca287c8c33e)
```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```
![download](https://github.com/user-attachments/assets/a4752b6e-a7ee-4dd6-b07c-ed26b55d7cf4)
![image](https://github.com/user-attachments/assets/c5790e68-dd9b-420a-9baf-7cf12c6842d2)
```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![download](https://github.com/user-attachments/assets/196e499b-2e28-4fb7-8377-9f8c8082aa43)
```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![download](https://github.com/user-attachments/assets/8ced1ca1-6ab4-41f4-86dc-d96592793cd2)
```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![download](https://github.com/user-attachments/assets/df372361-210c-4629-90fe-9a7de9c47dd9)



# Result:
Thus the program has been executed successfully.
