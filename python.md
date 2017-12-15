# Python

Snippets of python code I find myself looking up a lot. 

**Plot with matplotlib**

```python
import matplotlib.pyplot as plt

plt.plot(x_data_array,y_data_array, label='name of data')
plt.ylabel('y axis variable')
plt.xlabel('x axis variable')
plt.title('informative title')
plt.legend()
plt.show()
```

**Fun one liner**

```python
data = [1,2,3,4,5,6]
evens = [i for i in data if i%2==0]
```
