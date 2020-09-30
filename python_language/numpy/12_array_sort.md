Sorting an Array, which means putting element in order. we can use sort() to sort the element  like numeric or alphabetical, ascending or descending.
Eg:		import numpy as np
			arr = np.array([3, 2, 0, 1])

			print(np.sort(arr)) # which returns [0, 1, 2, 3]

If we want to sort the element alphabetically
Eg:		import numpy as np
			arr = np.array(['banana', 'cherry', 'apple'])

			print(np.sort(arr)) # which returns [''apple', banana', 'cherry']

Sorting 2-D Array
Eg:		import numpy as np
			arr = np.array([[3, 2, 4], [5, 0, 1]])

			print(np.sort(arr))
			# which returns
				[2, 3, 4]
				[0, 1, 5]

