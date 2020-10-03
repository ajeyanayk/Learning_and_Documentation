# Spliting an Arrays

* If we want to split the arrays two or more arrays, we can use the function **array_split()** <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5, 6, 7])```	 <br />
			```newarr = np.array_split(arr, 3)``` *which want to split the array into 3 arrays*  <br />
			```print(newarr)``` *which display* **[array([1, 2]),array([3, 4]),array([5, 6]),** 

* If the array has less elements than required, it will adjust from the end. <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5, 6])``` <br />
			```newarr = np.array_split(arr, 4)``` <br />
			```print(newarr)``` *which display* **[array([1, 2]),array([3, 4]),array([ 5 ])array([ 6]),**

* If we want to display the split arrays into line by line, We can use index method <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5, 6])``` <br />
			```newarr = np.array_split(arr, 3)``` <br />
			```print(newarr[0])``` <br />
			```print(newarr[1])``` <br />
			```print(newarr[2])``` <br />
			*which display* <br />
				**[1, 2]** <br />
				**[3, 4]** <br />
				**[ 5 ]** <br />
				**[ 6]**

 **Splitting 2-D Arrays**
 
* We need to use array_split() function to split 2-D Arrays  <br />
	*Eg 1*:	```import numpy as np``` <br />
			```arr = np.array([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10], [11, 12]])``` <br />
			```newarr = np.array_split(arr, 3)``` <br />
			```print(newarr)``` <br />
			*which display three  2-D Arrays*  <br />
			**[array([[1 2],[3 4]]), array([[5, 6],[7, 8]]), array([[9, 10],[11, 12]])]**

	*Eg 2*:	```import numpy as np``` <br />
			```arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12], [13, 14, 15], [16, 17, 18]])``` <br />
			```newarr = np.array_split(arr, 3)``` <br />
			```print(newarr)``` <br />
			*which display three  2-D Arrays*  <br />
			**[array([[1, 2, 3],[4, 5, 6]]), array([[7, 8, 9],[10, 11, 12]]), array([[13, 14, 15],[16, 17, 18]])]**

* We can split the array using **hsplit()** or **hstack()** method <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12], [13, 14, 15], [16, 17, 18]])``` <br />
			```newarr = np.hsplit(arr, 3)``` <br />
			```print(newarr)``` <br />
			*which display three  2-D Arrays* <br />
					**[array([[ 1],** <br />
					**[ 4],** <br />
					**[ 7],** <br />
					**[10],** <br />
					**[13],** <br />
					**[16]]), array([[ 2],** <br />
					**[ 5],** <br />
					**[ 8],** <br />
					**[11],** <br />
					**[14],** <br />
					**[17]]), array([[ 3],** <br />
					**[ 6],** <br />
					**[ 9],** <br />
					**[12],** <br />
					**[15],** <br />
					**[18]])]**

				