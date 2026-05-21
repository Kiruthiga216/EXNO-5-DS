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
x_val = [0,1,2,3,4,5]
y_val = [0,1,4,9,16,25]
plt.plot(x_val,y_val)
plt.show()

```

<img width="763" height="576" alt="image" src="https://github.com/user-attachments/assets/39d7ff80-11fa-41f5-b16f-6071169f3b69" />


```
import matplotlib.pyplot as plt
x = [1,2,3]
y = [2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My first graph')
plt.show()

```


<img width="819" height="623" alt="image" src="https://github.com/user-attachments/assets/85002f8d-593f-45f8-893b-77609e5672c0" />

```
import matplotlib.pyplot as plt
x1 = [1,2,3]
y1 = [2,5,3]
plt.plot(x1,y1,label = 'line 1')
x2 = [1,2,3]
y2 = [3,1,6]
plt.plot(x2,y2,label = 'line 2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("Two lines on the same graph")
plt.legend()
plt.show()
```

<img width="779" height="608" alt="image" src="https://github.com/user-attachments/assets/3d1b5b62-63b1-4964-a181-7bacb373fa4e" />


```
import matplotlib.pyplot as plt
import numpy as np
x = [1,2,3,4,5]
y1 = [10,12,14,16,18]
y2 = [5,7,9,11,13]
y3 = [2,4,6,8,10]
plt.fill_between(x,y1,color = 'blue')
plt.fill_between(x,y2,color = 'orange')

```

<img width="785" height="572" alt="image" src="https://github.com/user-attachments/assets/58395aa7-37fb-4d6f-832f-586aa949612b" />

```
plt.stackplot(x,y1,y2,y3,labels = ['line1','line2','line3'])
plt.legend(loc = 'upper left')
plt.title('Stacked line charts')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()

```

<img width="792" height="634" alt="image" src="https://github.com/user-attachments/assets/ab3ffe24-6963-4266-8355-3bab0a3c886d" />


```
import numpy as np
import matplotlib.pyplot as plt
val = [2,4,7,3]
names = ['A','B','C','D']
plt.bar(names, val,color = 'purple')
plt.show()

```

<img width="745" height="576" alt="image" src="https://github.com/user-attachments/assets/76b55e33-7961-408e-b85d-452cbfe99403" />


```
import matplotlib.pyplot as plt
import numpy as np
ages = [2,6,4,12,13,12,16,18,18,19,26,24,39,34,45,42,54,56,90,56,86,79]
range = (0,100)
bins = 10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no of people')
plt.title('histogram')
plt.show()

```

<img width="795" height="619" alt="image" src="https://github.com/user-attachments/assets/5ee8d0c8-b498-4a5f-ba14-5e928d892657" />


```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data

```

<img width="817" height="514" alt="image" src="https://github.com/user-attachments/assets/b968f560-766b-4d78-98b9-303394a146a3" />

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel("data")
ax.set_ylabel("values")
ax.set_title("box plot")

```

<img width="875" height="655" alt="image" src="https://github.com/user-attachments/assets/d531952f-b3a1-4807-9159-4ddcac26d8d0" />

```

import matplotlib.pyplot as plt
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels = slices,colors=colors,startangle=90,shadow = True,explode = (0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()

```

<img width="583" height="567" alt="image" src="https://github.com/user-attachments/assets/428941c5-ccb5-41af-9b4b-01a611db9fda" />




# Result:

Thus, We have successfullu performed Data Visualization using matplot python library for the given datas.
