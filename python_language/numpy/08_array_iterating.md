# Array Iteration

**3rd Iteration means going through each element**

+ Iterating 1-D Array <br />
	*Eg*: ```import numpy as np``` <br />
		  ```arr = np.array([1, 2, 3])``` <br />
			```for x in arr:``` <br />
  				```print(x)``` <br />
		 *which display the value as* <br />
					**1** <br />
					**2** <br />
					**3**

+ Iterating 2-D Arrays <br />
	*Eg*: ```import numpy as np``` <br />
		  ```arr = np.array([[1, 2, 3], [4, 5, 6]])``` <br />
		  ```for x in arr:``` <br />
		  		```print(x)``` <br />
			*which display the value as* <br />
					**[1 2 3]** <br />
					**[4 5 6]** 

+ If we want to iterate 2-D Arrays as 1-D array <br />
	*Eg*: ````import numpy as np``` <br />
		  ```arr = np.array([[1, 2, 3], [4, 5, 6]])``` <br />
		  ```for x in arr:``` <br />
		  		```for y in x:``` <br />
		    			```print(y)``` <br />
			*which display the value as* <br />
					  **1** <br />
					  **2** <br />
					  **3** <br />
					  **4** <br /> 
					  **5** <br />
					  **6**

+ Iterating 3-D Arrays <br />
	*Eg*: ```import numpy as np``` <br />
		  ```arr = np.array([[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]]])``` <br />
		  ```for x in arr:``` <br />
		  		```print(x)``` <br />
		   *which display as* <br />
		**x represents the 2-D array:** <br />
        **[[1 2 3]** <br />
        ** [4 5 6]]** <br />
		**x represents the 2-D array:** <br />
        **[[ 7  8  9]** <br />
         **[10 11 12]]** 

+ If we want to iterate 3-D Arrays as 1-D array <br />
	*Eg*: ```import numpy as np``` <br />
		  ```arr = np.array([[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]]])``` <br />
		  ```for x in arr:``` <br />
		  		```for y in x:``` <br />
		    		```for z in y:``` <br />
		      				```print(z)```

+ we can iterate the array by using the  function nditer(), which helps from basic to advance iteration <br />
	*Eg*: ```import numpy as np``` <br />
		  ```arr = np.array([[[1, 2], [3, 4]], [[5, 6], [7, 8]]])``` <br />
		  ```for x in np.nditer(arr):``` <br />
		  		```print(x)```, *Which displays 1-D array using nditer()*

**Iterating Array with different Data Types** - We can use op_dtypes arguments with datatype which is expected to change while iterating.
		
+ NumPy does not change the data type of the element in-place (where the element is in array) so it needs some other space to perform this action, that extra space is called buffer, and in order to enable it in nditer() we pass flags = ['buffered'] <br />
	*Eg*: ```import numpy as np``` <br />
		  ```arr = np.array([1, 2, 3])``` <br />
		  ```for x in np.nditer(arr, flags=['buffered'], op_dtypes=['S']):``` <br />
				```print(x)``` <br />
			*which displays* <br />
				**b'1'** <br />
				**b'2'** <br />
				**b'3'**
 
+ Iterating with different Step Size -  if we want to display the element in customized way Eg: Alternative element, every 3rd element etc. <br />
	*Eg*:  ```import numpy as np``` <br />
		   ```arr = np.array([[1, 2, 3, 4], [5, 6, 7, 8]])``` <br />
			```for x in np.nditer(arr[:, ::2]):``` <br />
		  		```print(x)``` *which display every alternative element in array while iterating* 

+ **Enumerated Iteration** -  If we want to the know the value with index, we can use ndenumerate() method <br />
	*Eg 1*:  ```import numpy as np``` <br />
			 ```arr = np.array([1, 2, 3])``` <br />
			  ```for idx, x in np.ndenumerate(arr):``` <br />
			 		```print(idx, x)``` *Here idx is index with array* <br />
				*which displays the value as* <br />
					**(0,)  1** <br />
					**(1,)  2** <br />
					**(2,)  3**

	*Eg 2*:   ```import numpy as np``` <br />
			  ```arr = np.array([[1, 2, 3, 4], [5, 6, 7, 8]])``` <br />
			  ```for idx, x in np.ndenumerate(arr):``` <br />
			  		```print(idx, x)``` *Here idx is index and x is element* <br />
				which displays the value as <br />
					**(0,0) 1** <br />
					**(0,1) 2** <br />
					**(0,2) 3** <br />
					**(0,3) 4** <br />		
					**(1,0) 5** <br />
					**(1,1) 6** <br />
					**(1,2) 7** <br />
					**(1,3) 8**
