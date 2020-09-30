If we want to search a certain value in Array, we can use where() method. which returns the index  number of the array
Eg 1:		import numpy as np
			arr = np.array([1, 2, 3, 4, 5, 4, 4])

			x = np.where(arr == 4)
			print(x) # which returns array([3, 5, 6]),) as the value in 3, 5 ,6 index

Eg 2: 	#Find the indexes where the values are even:
			import numpy as np
			arr = np.array([1, 2, 3, 4, 5, 6, 7, 8])

			x = np.where(arr%2 == 0)
			print(x) # which returns array([1, 3, 5, 7]),) as the even value in 1,3,5,7

Eg 3:	#Find the indexes where the values are odd:
			import numpy as np
			arr = np.array([1, 2, 3, 4, 5, 6, 7, 8])

			x = np.where(arr%2 == 1)
			print(x) # which returns array([0,2,4,6]),) as the odd value in 0,2,4,6

 Search Sorted - here is a method called searchsorted() which performs a binary search in the array, and returns the index where the specified value would be inserted to maintain the search order.
Eg:		import numpy as np
			arr = np.array([6, 7, 8, 9])

			x = np.searchsorted(arr, 7)
			print(x) #which returns value as 1
			#The number 7 should be inserted on index 1 to remain the sort order.
The method starts the search from the left and returns the first index where the number 7 is no longer larger than the next value.

Search from the Right side 
By default the left most index is returned, but we can give side='right' to return the right most index instead.
Eg:		import numpy as np
			arr = np.array([6, 7, 8, 9])

			x = np.searchsorted(arr, 7, side='right')
			print(x)#which returns value as 2
		#The number 7 should be inserted on index 2 to remain the sort order.
The method starts the search from the right and returns the first index where the number 7 is no longer less than the next value.

Multiple Values -  we can search more than one values in array using serachsorted()
Eg:		import numpy as np
			arr = np.array([1, 3, 5, 7])

			x = np.searchsorted(arr, [2, 4, 6])
			print(x)
			#The return value is an array: [1,2,3] containing the three indexes where 2, 4, 6 would be , inserted in the original array to maintain the order.

	