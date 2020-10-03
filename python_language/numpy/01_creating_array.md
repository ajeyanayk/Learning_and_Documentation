# Creating ndarray using Numpy

+ **Create a NumPy ndarray Object** - The array in Numpy is called ndarray. and which can create by using array() function. <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5])``` <br />
			```print(arr)#[1 2 3 4]``` <br />
			```print(type(arr)) <class 'numpy.ndarray'>```

**type()** : This built-in Python function tells us the type of the object passed to it. Like in above code it shows that arr is numpy.ndarray type.

#### Dimensions in Arrays -  A dimension in arrays is one level of array depth

+ **0-D arrays**: 0-D arrays or scalars are the elements in an array. <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array(42)``` *Single element in ndarray is called 0-D arrays* <br />
			```print(arr)```

+ **1-D arrays** :  an array has more than one 0-D arrays as it's element is called uni-dimension or 1-D array. <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5])``` *which has more than one 0-D arrays as its element* <br />
			```print(arr)``` 

+ **2-D arrays** :  an array an array has more than one 1-D arrays as it's element is called a 2-D array and these are used to represent <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([[1, 2, 3], [4, 5, 6]])``` <br />
			*which has more than one 1-D arrays as its element* <br />
			```print(arr)```

*NumPy has a whole sub module dedicated towards matrix operations called numpy.mat*

+ **3-D arrays** :  an array an array has more than one 2-D arrays as it's element is called a 3-D array. <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([[[1, 2, 3], [4, 5, 6]], [[1, 2, 3], [4, 5, 6]]])``` <br />
			```print(arr)```

**Check Number of Dimensions**

* We can check how many dimensions the array have  by using ndim method, which returns the value in Integer <br />
	*Eg*:	```import numpy as np``` <br />
			```a = np.array(42)``` <br />
			```b = np.array([1, 2, 3, 4, 5])``` <br />
			```c = np.array([[1, 2, 3], [4, 5, 6]])``` <br />
 			```d = np.array([[[1, 2, 3], [4, 5, 6]], [[1, 2, 3], [4, 5, 6]]])``` <br />
			```print(a.ndim)``` *which displays  0 as it is 0-D dimension* <br />
			```print(b.ndim)``` *which displays  1 as it is 1-D dimension* <br />
			```print(c.ndim)``` *which displays  2 as it is 2-D dimension* <br /> 
			```print(d.ndim)``` *which displays 3 as it is 3-D dimension*

**Higher Dimensional Arrays**

* Once arrays is created , we can define the number of dimension using ndmin argument <br />
	*Eg*:	*Creating 5 dimension array and verifying* <br />
			```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4], ndmin=5)``` <br />
			```print(arr) #[[[[[1 2 3 4]]]]]``` <br />
			```print('number of dimensions :', arr.ndim)``` *number of dimension : 5*

