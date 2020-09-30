Array Reshape, means reshaping we can add or remove dimension or change number of elements in each dimension. We can reshape the element using reshape() method.

Reshape from 1-D to 2-D - Converting  1-D array element to 2-D array, 
Eg:		import numpy as np
			arr = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])
			newarr = arr.reshape(4, 3)#Here 4 indicates Arrays and 3 is element on those arrays

			print(newarr) 
			# which returns
			[[1  2  3]
			  [4 5  6]
			  [7	8	9]
			  [10 11  12]]

Reshape from 1-D to 3-D - Converting  1-D array element to 3-D array,
Eg:		import numpy as np
			arr = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])
			newarr = arr.reshape(2, 3, 2) 
#Here 2 indicates Arrays , 3 is  also from those 3 arrays and each arrays having 2 elements.

			print(newarr) 
			#which returns
			[[[1	2]
			   [3  4]
			   [5   6]]

			   [7  8]
			   [9  10]
			   [11  12]]]

The reshape method is View, we can identify this  by using  base() method
Eg:		import numpy as np
			arr = np.array([1, 2, 3, 4, 5, 6, 7, 8])

			print(arr.reshape(2, 4).base) # which returns the value as original [ 1 2 3 4 5 6 7 8]

Unknown Dimension
 If the elements in 1-D are unknown, we can specify -1 with dimension, Python we check and make the array according to element . If not possible it will return with error message
Eg:		import numpy as np
			arr = np.array([1, 2, 3, 4, 5, 6, 7, 8])
			newarr = arr.reshape(2, 2, -1)

			print(newarr)
			#which returns
			[[1	2]
			  [3  4]]

			  [5  6]
			  [7  8]]

Flattering the arrays-   which converts multidimensional array into 1-D Array
Eg:		import numpy as np
			arr = np.array([[1, 2, 3], [4, 5, 6]])

			newarr = arr.reshape(-1)
			print(newarr) # which returns [1 2 3 4 5 6]