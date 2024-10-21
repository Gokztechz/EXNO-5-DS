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
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/1bff390d-1e13-4130-a4c0-bf206ab6777c)

'''
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
'''
![image](https://github.com/user-attachments/assets/0ac59afc-8a37-46ac-8e53-769ebacfea9a)
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
![image](https://github.com/user-attachments/assets/5d843b6f-909c-4ebd-ad4f-6c5c0c56b752)
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
![image](https://github.com/user-attachments/assets/c0f93092-6c54-4c12-bba4-d930513797a0)
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);
![image](https://github.com/user-attachments/assets/731a3080-3b93-4e49-a11d-03771ff96acf)
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
![image](https://github.com/user-attachments/assets/20fd9119-b82a-4b6a-8d78-b3e1c9b2672b)
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
![image](https://github.com/user-attachments/assets/231bc848-964e-4e4b-9325-64c8f87b4456)
y
![image](https://github.com/user-attachments/assets/84be516a-9adb-4b8a-afa9-66284ccbfc6f)
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
![image](https://github.com/user-attachments/assets/6c704c92-72ec-4604-936c-9f7f4f3a67cb)
y=x*x
y
![image](https://github.com/user-attachments/assets/bb38a363-08f3-46c2-8700-a303f343a086)
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
![image](https://github.com/user-attachments/assets/76dede53-fb9e-454b-93fc-43833770db13)
np.pi
![image](https://github.com/user-attachments/assets/9d656eaf-367e-47ec-ae0d-e5369b79738f)
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
![image](https://github.com/user-attachments/assets/9dc687ea-39fd-4a9a-8375-a3473bcb486f)
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
![image](https://github.com/user-attachments/assets/b3c73545-f193-4ed0-ad2e-bb1ab5100b29)
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
![image](https://github.com/user-attachments/assets/1832ab8c-6055-4e88-bca6-60b055986d9e)
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
![image](https://github.com/user-attachments/assets/30efb37a-e407-4761-8e9b-720aabc73255)
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
![image](https://github.com/user-attachments/assets/262b664c-b471-4cbc-93da-aa9d7c5f9117)
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
![image](https://github.com/user-attachments/assets/4493aafc-9f5f-4010-b0d2-889c75f235c0)
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
![image](https://github.com/user-attachments/assets/8a0e812a-2ddf-47e1-ad54-c25f4ac4a541)
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
![image](https://github.com/user-attachments/assets/1f0790e3-5785-4c19-a010-d9c11e7ce1a4)
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
![image](https://github.com/user-attachments/assets/dd4acc87-b46d-4373-972b-8e844aebced3)
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
![image](https://github.com/user-attachments/assets/1ed9a474-f629-4313-a8de-902f526df944)




 

# Result:
 Thus, The implementation of data visualization using matplotlib has been successfully verified.


