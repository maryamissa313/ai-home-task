# ai-home-task
what is numpy?
numpy is a python libarary used for working with arrays.used for numerical computing.
it provides support for multi_dimensional arrays and matrices<along with mathematical
functions to operate these structures efficiently.

why use numpy?
fasrer thanpython lists
uses less memory
provides built_in functions for complex mathematical operations.
supports multi-dimensional arrays and matrices

why is numpy faster than lists?
numpy arrays are stored at one continuous place in memory unlike lists,so processes
can access and manipulate them very efficently.
import numpy as np
import time
size=1_000_000
list_data=list(range(size))
start_time=time.time()
sum_list=sum(list_data)
end_time=time.time()
list_time=end_time-start_time
np_data=np.array(size)
start_time=time.time()
sum_np=np.sum(np_data)
end_time=time.time()
np_time=end_time-start_time
print(f"time taken by list:{list_time}")
print(F"timetaken by numpy:{np_time}")

which language  is numpy written in?
numpy is a python libarary and written in python,c and c++.

installation of numpy?
pip install numpy
import numpy as np

dimensions in array
there is zero, one ,two, three and nd arrays in numpy
example
a = np.array(42)
b = np.array([1, 2, 3, 4, 5])
c = np.array([[1, 2, 3], [4, 5, 6]])
d = np.array([[[1, 2, 3], [4, 5, 6]], [[1, 2, 3], [4, 5, 6]]])

print(a.ndim)
print(b.ndim)
print(c.ndim)
print(d.ndim)

copy and view in numpy
in copy base remains same and in view base also change
copy

import numpy as np
arr = np.array([1, 2, 3, 4, 5])
x = arr.copy()
arr[0] = 42
arr[4] = 45
print(arr)
print(x)

view
import numpy as np
arr = np.array([1, 2, 3, 4, 5])
x = arr.view()
arr[0] = 42
arr[4] =32
print(arr)
print(x)

 join two arrays
    join two arrays by using concatenate

import numpy as np
arr1=np.array([1,2,3])
arr2=np.array([4,5,6])
new_arr=np.concatenate((arr1,arr2))
print("new_arr:",new_arr) 

joning array using stack function
    stack also help to join array in different ways

arr1=np.array([1,2,3])
arr2=np.array([4,5,6])
v_stack=np.vstack((arr1,arr2))
print("stacked vertically:",v_stack)
h_stack=np.hstack((arr1,arr2))
print("stacked horizantally:",h_stack)
d_stack=np.dstack((arr1,arr2))
print("stacked depth:",d_stack)

spliting numpy array

   it splite a arrray in in different dimensional

arr=np.array([1,2,3,4,5,6])
split_arrays=np.array_split(arr,3)
print("splict array:",split_arrays)

searching in numpy arrays
    by using where function we search the index of an arrays

array1=np.array([1,2,3,4,5,6,3,4,5,6,3,3])
index=np.where(array1==3)
print("index of value 3 in array1:",index)



