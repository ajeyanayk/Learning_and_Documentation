3rd Iteration means going through each element

Iterating 1-D Array 
Eg:	import numpy as np
		arr = np.array([1, 2, 3])

		for x in arr:
  			print(x)
		# which display the value as 
						1
						2	
						3

Iterating 2-D Arrays
Eg:	import numpy as np
		arr = np.array([[1, 2, 3], [4, 5, 6]])

		for x in arr:
		  print(x)
		# which display the value as 
					[1 2 3]
					[4 5 6]

	If we want to iterate 2-D Arrays as 1-D array
Eg:	import numpy as np
		arr = np.array([[1, 2, 3], [4, 5, 6]])

		for x in arr:
		  for y in x:
		    print(y)
	# which display the value as 
						1
						2
						3
						4
						5
						6

Iterating 3-D Arrays
Eg:	import numpy as np
		arr = np.array([[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]]])

		for x in arr:
		  print(x)
		#which display as 
	x represents the 2-D array:
        [[1 2 3]
          [4 5 6]]
    x represents the 2-D array:
        [[ 7  8  9]
         [10 11 12]]

If we want to iterate 3-D Arrays as 1-D array
Eg:	import numpy as np
		arr = np.array([[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]]])

		for x in arr:
		  for y in x:
		    for z in y:
		      print(z)

we can iterate the array by using the  function nditer(), which helps from basic to advance iteration
Eg:	import numpy as np
		arr = np.array([[[1, 2], [3, 4]], [[5, 6], [7, 8]]])

		for x in np.nditer(arr):
		  print(x), Which displays 1-D array using nditer()

 Iterating Array with different Data Types
	We can use op_dtypes arguments with datatype which is expected to change while 	iterating.
		NumPy does not change the data type of the element in-place (where the element is in array) so it needs some other space to perform this action, that extra space is called buffer, and in order to enable it in nditer() we pass flags = ['buffered']
Eg:	import numpy as np
		arr = np.array([1, 2, 3])

		for x in np.nditer(arr, flags=['buffered'], op_dtypes=['S']):
		  print(x)
		# which displays
				b'1'
				b'2'
				b'3'
 
Iterating with different Step Size -  if we want to display the element in customized way Eg: Alternative element, every 3rd element etc.
Eg:	import numpy as np
		arr = np.array([[1, 2, 3, 4], [5, 6, 7, 8]])

		for x in np.nditer(arr[:, ::2]):
		  print(x) # which display every alternative element in array while iterating

Enumerated Iteration -  If we want to the know the value with index, we can use ndenumerate() method
Eg 1:		import numpy as np
			arr = np.array([1, 2, 3])

			for idx, x in np.ndenumerate(arr):
			  print(idx, x) # Here idx is index with array
			# which displays the value as 
					(0,)  1
					(1,)  2
					(2,)  3

Eg 2: 	import numpy as np
			arr = np.array([[1, 2, 3, 4], [5, 6, 7, 8]])

			for idx, x in np.ndenumerate(arr):
			  print(idx, x) Here idx is index and x is element
			# which displays the value as 
					(0,0) 1
					(0,1)  2
					(0,2) 3
					(0,3) 4					
					(1,0) 5
					(1,1) 6
					(1,2)7
					(1,3)8
