The difference between Copy and View is
Copy is the copy of the original array, which owns the data and we can change the data  without affecting the original array.
View is the view of the original, which owns the data. If we are changing the data in view array it affect on original array and vice versa. 

Copy -  we can make a copy array by using copy() method and if we change the original array which doesn't affect on copy file
Eg:		import numpy as np
			arr = np.array([1, 2, 3, 4, 5])
			x = arr.copy()
			arr[0] = 42 # change was done in original array
		
			print(arr) # displays original array - [42, 2, 3, 4, 5]
			print(x)	 # displays copy of original array - [1, 2, 3, 4, 5] 

View - we can make a view, using view() method and if we change the original array which affects on view array
Eg 1:		import numpy as np
			arr = np.array([1, 2, 3, 4, 5])
			x = arr.view()
			arr[0] = 42 # change was done in original array
			
			print(arr) # displays original array - [42, 2, 3, 4, 5]
			print(x) # displays view array - [42, 2, 3, 4, 5]

Eg 2:	import numpy as np
			arr = np.array([1, 2, 3, 4, 5])
			x = arr.view()
			x[0] = 31 # change was done in view array

			print(arr) # displays original array - [31, 2, 3, 4, 5]
			print(x) # displays view array - [31, 2, 3, 4, 5]

check if Array own it's data - we can check Array owns data by using base() method, Here base refers to original file.
Eg:		import numpy as np
			arr = np.array([1, 2, 3, 4, 5])
			x = arr.copy()
			y = arr.view()
			
			print(x.base) # which returns as "None" which has its own data
			print(y.base) # which displays [1, 2, 3, 4, 5]