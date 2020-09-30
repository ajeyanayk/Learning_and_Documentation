If we want to split the arrays two or more arrays, we can use the function array_split()
Eg:	import numpy as np
		arr = np.array([1, 2, 3, 4, 5, 6, 7])
		
		newarr = np.array_split(arr, 3) # which want to split the array into 3 arrays 
		print(newarr) # which display [array([1, 2]),array([3, 4]),array([5, 6]), 

If the array has less elements than required, it will adjust from the end.
Eg:		import numpy as np
			arr = np.array([1, 2, 3, 4, 5, 6])

			newarr = np.array_split(arr, 4)
			print(newarr) # which display [array([1, 2]),array([3, 4]),array([ 5 ])array([ 6]), 

If we want to display the split arrays into line by line, We can use index method
Eg:		import numpy as np
			arr = np.array([1, 2, 3, 4, 5, 6])

			newarr = np.array_split(arr, 3)
			print(newarr[0])
			print(newarr[1])
			print(newarr[2])
			# which display
				[1, 2]
				[3, 4]
				[ 5 ]
				[ 6]

  Splitting 2-D Arrays
We  need to use array_split() function to split 2-D Arrays 
Eg 1:		import numpy as np
			arr = np.array([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10], [11, 12]])
			
			newarr = np.array_split(arr, 3)
			print(newarr)
			# which display three  2-D Arrays 
			[array([[1 2],[3 4]]), array([[5, 6],[7, 8]]), array([[9, 10],[11, 12]])]

Eg 2:	import numpy as np
			arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12], [13, 14, 15], [16, 17, 18]])

			newarr = np.array_split(arr, 3)
			print(newarr)
			# which display three  2-D Arrays 
			[array([[1, 2, 3],[4, 5, 6]]), array([[7, 8, 9],[10, 11, 12]]), array([[13, 14, 15],[16, 17, 18]])]

 We can split the array using hsplit() or hstack() method
Eg:		import numpy as np
			arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12], [13, 14, 15], [16, 17, 18]])

			newarr = np.hsplit(arr, 3)
			print(newarr)
		# which display three  2-D Arrays 
[array([[ 1],
       [ 4],
       [ 7],
       [10],
       [13],
       [16]]), array([[ 2],
       [ 5],
       [ 8],
       [11],
       [14],
       [17]]), array([[ 3],
       [ 6],
       [ 9],
       [12],
       [15],
       [18]])]

				