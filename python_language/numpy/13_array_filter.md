Removing some element from existing and creating a new array is called Filtering. 

 In Numpy, we can filter an array using a boolean index list

If the value at an index is True that element is contained in the filtered array, if the value at that index is False that element is excluded from the filtered array.

Eg:		import numpy as np
			arr = np.array([41, 42, 43, 44])

			x = arr[[True, False, True, False]]
			print(x) # which displays [41, 43]

Creating the Filter Array - creating the Filter based on condition
Eg 1:		import numpy as np
			arr = np.array([41, 42, 43, 44])

			# Create an empty list
			filter_arr = []

			# go through each element in arr
			for element in arr:
			  # if the element is higher than 42, set the value to True, otherwise False:
			  if element > 42:
			    filter_arr.append(True)
			  else:
			    filter_arr.append(False)

			newarr = arr[filter_arr]
			print(filter_arr)# which displays [False False True True]
			print(newarr) # which displays [43, 44]

Eg 2:	import numpy as np
			arr = np.array([1, 2, 3, 4, 5, 6, 7])
			
			# Create an empty list
			filter_arr = []

			# go through each element in arr
			for element in arr:
 			 # if the element is completely divisble by 2, set the value to True, otherwise False
			  if element % 2 == 0:
			    filter_arr.append(True)
			  else:
			    filter_arr.append(False)

			newarr = arr[filter_arr]
			print(filter_arr)# which displays [False, True,False, True,False, True,False]
			print(newarr) # which displays [2, 4, 6]

Creating Filter Directly from Array
Eg 1:		#Create a filter array that will return only values higher than 42
			import numpy as np
			arr = np.array([41, 42, 43, 44])

			filter_arr = arr > 42

			newarr = arr[filter_arr]
			print(filter_arr)# which displays [False False True True]
			print(newarr) # which displays [43, 44]

Eg 2:	#Create a filter array that will return only even elements from the original array
			import numpy as np
			arr = np.array([1, 2, 3, 4, 5, 6, 7])

			filter_arr = arr % 2 == 0
			newarr = arr[filter_arr]
				print(filter_arr)# which displays [False, True,False, True,False, True,False]
			print(newarr) # which displays [2, 4, 6]
c