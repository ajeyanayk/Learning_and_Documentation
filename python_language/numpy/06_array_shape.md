Array shape , which means the number element in each dimension and we can find by using shape() method.
Eg  1:		import numpy as np
				arr = np.array([[1, 2, 3, 4], [5, 6, 7, 8]])

				print(arr.shape) #returns (2,4), here 2 is dimension and 4 is elements in each dim.

Eg 2:		import numpy as np
				 # creating an array with 6 dimension
				arr = np.array(([[1, 2, 3, 4], [5, 6, 7, 8]]), ndmin=6)

				print(arr)
				# which displays
				[[[[[[1 2 3 4]
						[5 6 7 8]]]]]]
				print('shape of array :', arr.shape) 
				# returns shape of array : (1, 1, 1, 1, 2, 4)
				


 