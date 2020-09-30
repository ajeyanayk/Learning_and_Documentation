we can join Two or more Numpy arrays using Concatenate() function along with the axis.  If axis is not mentioned it will take 0 as default
Eg 1:		import numpy as np
			arr1 = np.array([1, 2, 3])
			arr2 = np.array([4, 5, 6])

			arr = np.concatenate((arr1, arr2))
			print(arr)  # which displays as [1 2 3	4	5	6 ]

Eg 2:	import numpy as np
			arr1 = np.array([[1, 2], [3, 4]])
			arr2 = np.array([[5, 6], [7, 8]])

			arr = np.concatenate((arr1, arr2), axis=1)
			print(arr)
			# which displays as 
			[[1  2 5	6 ]
			  [3 4 7 8 ]]

Joining Arrays Using Stack Functions
Stacking is same as concatenate of two or more Arrays, along with axis
We can concatenate two 1-D arrays along the second axis which would result in putting them one over the other, ie. stacking.
Eg:		import numpy as np
			arr1 = np.array([1, 2, 3])
			arr2 = np.array([4, 5, 6])

			arr = np.stack((arr1, arr2), axis=1)
			print(arr)
			# which displays as 
				[1 4]
				[2 5]
				[3 6]

Stacking Along Rows
We can stack the element using hstack()
Eg:  		import numpy as np
			arr1 = np.array([1, 2, 3])
			arr2 = np.array([4, 5, 6])

			arr = np.hstack((arr1, arr2))
			print(arr) # which displays [ 1 2 3 4 5 6]

Stacking Along  columns
we can stack the element using vstack()
Eg:		import numpy as np
			arr1 = np.array([1, 2, 3])
			arr2 = np.array([4, 5, 6])

			arr = np.vstack((arr1, arr2))
			print(arr)
			# which displays as 
				[1 2 3]
				[4 5 6]

Stacking Along  Height depth
If we want to stack the array along with height, we can use dstack() method
Eg:		import numpy as np
			arr1 = np.array([1, 2, 3])
			arr2 = np.array([4, 5, 6])

			arr = np.dstack((arr1, arr2))
			print(arr)
			# which displays as 
				[[1 4]
				 [2 5]
				 [3 6]]

		


