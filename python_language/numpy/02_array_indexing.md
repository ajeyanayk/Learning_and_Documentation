# Accessing Element from Array using Numpy in python

**Access Array Elements**

* We can access the element in  Numpy arrays by referring to its index number.<br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4])``` <br />
			```print(arr[0])``` *which displays value as 1* 

* Get third and fourth elements from the following array and add them <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4])``` <br />
			```print(arr[2] + arr[3])``` <br />
*which displays the value 7 as 3rd element is 3 & 4th element is 4*

* Access 2-D Arrays -  we can access 2-D arrays by referring 1 dimension and 1 index of element by separting commas. <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([[1,2,3,4,5], [6,7,8,9,10]])``` <br />
			```print('2nd element on 1st dim: ', arr[0, 1])``` <br />
			*which displays as 2nd element on 1st dim:2* <br />
			```arr1 = np.array([[1,2,3,4,5], [6,7,8,9,10]])``` <br />
			```print('5th element on 2nd dim: ', arr[1, 4])``` <br />
			*which displays as 5th element on 2nd dim: 10

* Access 3-D Arrays -  we can access 3-D arrays by 1 dimension and 2 index of elements by separating commas <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]], [[13, 14, 15], [16, 17, 18]]])``` <br />
			```print(arr[0, 1, 2])``` # which returns 6 <br />
			**"""arr[0, 1, 2]** prints the value 6. <br />
			The first number represents the first dimension, which contains two arrays: <br />
			**[[1, 2, 3], [4, 5, 6]]**  and       **[[7, 8, 9], [10, 11, 12]]** <br />
			Since we selected 0, we are left with the first array: <br />
			**[[1, 2, 3], [4, 5, 6]]** <br />
			The second number represents the second dimension, it also contains two arrays: <br />
			**[1, 2, 3]**   and      **[4, 5, 6]** <br />
			Since we selected 1, we are left with the second array: <br />
			**[4, 5, 6]** <br />
			The third number represents the third dimension, it contains three values: <br />
						**4** <br />
						**5** <br />
						**6** <br />
			Since we selected 2, we end up with the third value:6 """ <br />
			```print(arr[1, 1, 1])``` *which returns 11* <br />
			```print(arr[2, 0, 2])``` *which returns 15* 

+ **Negative Indexing** : we can use negative index to access element in an array from end <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([[1,2,3,4,5], [6,7,8,9,10]])``` <br />
			```print('Last element from 2nd dim: ', arr[1, -1])``` *which returns the value 10*






