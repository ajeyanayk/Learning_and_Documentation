# Array Reshape

+ **Array Reshape**, means reshaping we can add or remove dimension or change number of elements in each dimension. We can reshape the element using **reshape()** method.<br />

+ *Reshape from 1-D to 2-D - Converting  1-D array element to 2-D array,* <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])``` <br />
			```newarr = arr.reshape(4, 3)``` *Here 4 indicates Arrays and 3 is element on those arrays* <br />
			```print(newarr)``` <br />
			*which returns* <br />
			```[[1  2  3]``` <br />
			  ```[4 5  6]``` <br />
			  ```[7	8	9]``` <br />
			  ```[10 11  12]]``` 

+ *Reshape from 1-D to 3-D - Converting  1-D array element to 3-D array,* <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])``` <br />
			```newarr = arr.reshape(2, 3, 2)``` <br />
*Here 2 indicates Arrays , 3 is  also from those 3 arrays and each arrays having 2 elements*. <br />
			```print(newarr)```  <br />
			*which returns* <br />
			```[[[1	2]``` <br />
			   ```[3  4]``` <br />
			   ```[5   6]]``` <br />
			   ```[7  8]``` <br />
			   ```[9  10]``` <br />
			   ```[11  12]]]``` 

+ The reshape method is View, we can identify this  by using  **base()** method <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5, 6, 7, 8])``` <br />
			```print(arr.reshape(2, 4).base)``` *which returns the value as original* **[ 1 2 3 4 5 6 7 8]**

**Unknown Dimension**

+ If the elements in 1-D are unknown, we can specify -1 with dimension, Python we check and make the array according to element . If not possible it will return with error message <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5, 6, 7, 8])``` <br />
			```newarr = arr.reshape(2, 2, -1)``` <br />
			```print(newarr)``` <br />
			*which returns* <br />		
			```[[1	2]``` <br />
			  ```[3  4]]``` <br />
			  ```[5  6]``` <br />
			  ```[7  8]]```

+ **Flattering the arrays** - which converts multidimensional array into 1-D Array <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([[1, 2, 3], [4, 5, 6]])```` <br />
			```newarr = arr.reshape(-1)``` <br />
			```print(newarr)``` *which returns* **[1 2 3 4 5 6]**