# Array Joining 

* we can join Two or more Numpy arrays using Concatenate() function along with the axis.  If axis is not mentioned it will take 0 as default <br />
	*Eg1*: ```import numpy as np``` <br />
		   ```arr1 = np.array([1, 2, 3])``` <br />
		   ```arr2 = np.array([4, 5, 6])``` <br />
		   ```arr = np.concatenate((arr1, arr2))``` <br />
		   ```print(arr)``` *which displays as* **[1 2 3	4	5	6 ]**

	*Eg2*: ```import numpy as np``` <br />
		   ```arr1 = np.array([[1, 2], [3, 4]])``` <br />
		   ```arr2 = np.array([[5, 6], [7, 8]])``` <br />
		   ```arr = np.concatenate((arr1, arr2), axis=1)``` <br />
		   ```print(arr)``` <br />
		    *which displays as* <br />
			**[[1  2 5	6 ]** <br />
			 **[3 4 7 8 ]]**

**Joining Arrays Using Stack Functions**

* Stacking is same as concatenate of two or more Arrays, along with axis <br />
	+ We can concatenate two 1-D arrays along the second axis which would result in putting them one over the other, ie. stacking. <br />
		*Eg*:  ```import numpy as np``` <br />
			   ```arr1 = np.array([1, 2, 3])``` <br />
			   ```arr2 = np.array([4, 5, 6])``` <br />
			   ```arr = np.stack((arr1, arr2), axis=1)``` <br />
			   ```print(arr)``` <br />
			*which displays as*  <br />
				**[1 4]** <br />
				**[2 5]** <br />
				**[3 6]**

**Stacking Along Rows** <br />

* We can stack the element using **hstack()* <br />
	*Eg*: ```import numpy as np``` <br />
		  ```arr1 = np.array([1, 2, 3])``` <br />
		  ```arr2 = np.array([4, 5, 6])``` <br />
		  ```arr = np.hstack((arr1, arr2))``` <br />
		  ```print(arr) # which displays [ 1 2 3 4 5 6]```	

**Stacking Along  columns**

* we can stack the element using **vstack()** <br />
	*Eg*: ```import numpy as np``` <br />
		  ```arr1 = np.array([1, 2, 3])``` <br />
		  ```arr2 = np.array([4, 5, 6])``` <br />
		  ```arr = np.vstack((arr1, arr2))``` <br />
		  ```print(arr)``` <br />
			*which displays as* <br />
			  **[1 2 3]** <br />
			  **[4 5 6]** 

**Stacking Along  Height depth**

* If we want to stack the array along with height, we can use **dstack()** method <br />
	*Eg*:  ```import numpy as np``` <br />
		   ```arr1 = np.array([1, 2, 3])``` <br />
		   ```arr2 = np.array([4, 5, 6])``` <br />
		   ```arr = np.dstack((arr1, arr2))``` <br />
		   ```print(arr)``` <br />
		   *which displays as* <br />
				**[[1 4]** <br />
				**[2 5]** <br />
				**[3 6]]** 

		


