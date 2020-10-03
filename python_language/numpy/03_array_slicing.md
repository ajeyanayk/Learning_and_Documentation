# Array Slicing using Numpy in Python

**Array slicing meaning taking elements from one index to new index.** <br />
*we can slice an array by* **[start:end]** or **[start: end :step]** <br />
*As default the value of step is 1 and which determine the increment in slicing* <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5, 6, 7])``` <br />
			```print(arr[1:5])``` //The result includes the start index, but excludes the end index*. <br />
				*which returns* **[ 2 3 4 5 ]** 

* If the start index is not mentioned, it consider from begging (its considering from 0). <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5, 6, 7])``` <br />
			```print(arr[4:])``` <br />
				*which returns* **[ 5 6 7 ]**

* If the end index is not mentioned, then it consider till end (its considered length of array in that dimension) <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5, 6, 7])``` <br />
			```print(arr[:4])``` // The result excludes the end index <br />
				*which returns* **[ 1 2 3 4 ]**

* Also Negative  <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5, 6, 7])``` <br />
			```print(arr[-3:-1])# The result excludes the end index``` <br />
				*which returns* **[ 5 6 ]**

* **Step**  -  The value determines, how many increment in index to be done while slicing <br />
	*Eg 1*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5, 6, 7])``` <br />
			```print(arr[1:5:2])``` <br />
				*which returns* **[ 2 4 ]** *as increment in index is* **2**

	*Eg 2*: *If Start or end is not mentioned and step is 2.* <br />
			```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4, 5, 6, 7])``` <br />
			```print(arr[::2])``` *which prints every alternative index in that array* 

* **Slicing 2-D array** -  we can slicing by defining element and rest as in above example <br />
	Syntax : ```[element, start:end:step]``` <br />
	*Eg 1*:  ```import numpy as np``` <br />
			 ```arr = np.array([[1, 2, 3, 4, 5], [6, 7, 8, 9, 10]])``` <br />
			 ```print(arr[1, 1:4])``` *element is [ 6, 7, 8, 9, 10 ] and the result display as* **[7 8 9 ]**

	*Eg 2*:	 ```import numpy as np``` <br />
			 ```arr = np.array([[1, 2, 3, 4, 5], [6, 7, 8, 9, 10]])``` <br />
			 ```print(arr[0:2, 2])``` *takes both elements as 0:2 and index 2 from both elements* <br />
				*the result is* **[3 8]**

	*Eg 3*:	 ```import numpy as np``` <br />
			 ```arr = np.array([[1, 2, 3, 4, 5], [6, 7, 8, 9, 10]])``` <br />
			 ```print(arr[0:2, 1:4])``` *takes both elements and index from 1:4 both elements* <br />
				*the result is* **[[2 3 4] [7 8 9]]**







