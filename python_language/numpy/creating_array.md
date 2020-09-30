Create a NumPy ndarray Object - The array in Numpy is called ndarray. and which can create by using array() function.
Eg:		import numpy as np
			arr = np.array([1, 2, 3, 4, 5])
			print(arr)#[1 2 3 4]
			print(type(arr)) <class 'numpy.ndarray'>
#type(): This built-in Python function tells us the type of the object passed to it. Like in above code it shows that arr is numpy.ndarray type.

Dimensions in Arrays -  A dimension in arrays is one level of array depth

0-D arrays: 0-D arrays or scalars are the elements in an array .
Eg:		import numpy as np
			arr = np.array(42) # Single element in ndarray is called 0-D arrays
			print(arr)

1-D arrays :  an array has more than one 0-D arrays as it's element is called uni-dimension or 1-D array.
Eg:		import numpy as np
			arr = np.array([1, 2, 3, 4, 5]) # which has more than one 0-D arrays as its element
			print(arr)

2-D arrays :  an array an array has more than one 1-D arrays as it's element is called a 2-D array and these are used to represent
Eg:		import numpy as np
			arr = np.array([[1, 2, 3], [4, 5, 6]])
			# which has more than one 1-D arrays as its element
			print(arr)
NumPy has a whole sub module dedicated towards matrix operations called numpy.mat

3-D arrays :  an array an array has more than one 2-D arrays as it's element is called a 3-D array.
Eg:		import numpy as np
			arr = np.array([[[1, 2, 3], [4, 5, 6]], [[1, 2, 3], [4, 5, 6]]])
			print(arr)

Check Number of Dimensions 
		We can check how many dimensions the array have  by using ndim method, which returns the value in Integer
Eg:		import numpy as np
			a = np.array(42) 
			b = np.array([1, 2, 3, 4, 5])
			c = np.array([[1, 2, 3], [4, 5, 6]])
			d = np.array([[[1, 2, 3], [4, 5, 6]], [[1, 2, 3], [4, 5, 6]]])

			print(a.ndim) # which displays  0 as it is 0-D dimension
			print(b.ndim)# which displays  1 as it is 1-D dimension
			print(c.ndim)# which displays  2 as it is 2-D dimension
			print(d.ndim)# which displays 3 as it is 3-D dimension

Higher Dimensional Arrays 
Once arrays is created , we can define the number of dimension using ndmin argument
Eg:		Creating 5 dimension array and verifying 
			import numpy as np
			arr = np.array([1, 2, 3, 4], ndmin=5)
			print(arr) #[[[[[1 2 3 4]]]]]
			print('number of dimensions :', arr.ndim) # number of dimension : 5

