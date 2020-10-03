# Filtering Array

**Removing some element from existing and creating a new array is called Filtering.** <br />

*In Numpy, we can filter an array using a boolean index list* <br />

* If the value at an index is True that element is contained in the filtered array, if the value at that index is False that element is excluded from the filtered array. <br />

	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([41, 42, 43, 44])``` <br />
			```x = arr[[True, False, True, False]]``` <br />
			```print(x) # which displays [41, 43]```

* Creating the Filter Array - creating the Filter based on condition <br />
	*Eg 1*:	```import numpy as np``` <br />
			```arr = np.array([41, 42, 43, 44])``` <br />
				*Create an empty list* <br />
					**filter_arr = []** <br />
				*go through each element in arr* <br />
				```for element in arr:``` <br />
				if the element is higher than 42, set the value to True, otherwise False: <br />
					```if element > 42:``` <br />
							```filter_arr.append(True)``` <br />
					```else:``` <br />
							```filter_arr.append(False)``` <br />
				```newarr = arr[filter_arr]``` <br />
				```print(filter_arr)``` *which displays* **[False False True True]** <br />
				```print(newarr)``` *which displays* **[43, 44]**

	*Eg 2*:		```import numpy as np``` <br />
				```arr = np.array([1, 2, 3, 4, 5, 6, 7])``` <br />
				*Create an empty list* <br />
				```filter_arr = []``` <br />
				*go through each element in arr* <br />
				```for element in arr:``` <br />
				**if the element is completely divisble by 2, set the value to True, otherwise False** <br />
				```if element % 2 == 0:``` <br />
					```filter_arr.append(True)``` <br />
				```else:``` <br />
					```filter_arr.append(False)``` <br />
				```newarr = arr[filter_arr]``` <br />
				```print(filter_arr)``` *which displays* **[False, True,False, True,False, True,False]** <br />
				```print(newarr)``` *which displays* **[2, 4, 6]**

* Creating Filter Directly from Array <br />
	*Eg 1*:		*Create a filter array that will return only values higher than 42* <br />
				```import numpy as np``` <br />
				```arr = np.array([41, 42, 43, 44])``` <br />
				```filter_arr = arr > 42``` <br />
				```newarr = arr[filter_arr]``` <br />
				```print(filter_arr)``` *which displays* **[False False True True]** <br />
				```print(newarr)``` *which displays* **[43, 44]**

	*Eg 2*:		*Create a filter array that will return only even elements from the original array* <br />
				```import numpy as np``` <br />
				```arr = np.array([1, 2, 3, 4, 5, 6, 7])``` <br />
				```filter_arr = arr % 2 == 0``` <br />
				```newarr = arr[filter_arr]``` <br />
				```print(filter_arr)``` *which displays* **[False, True,False, True,False, True,False]** <br />
				```print(newarr)``` *which displays* **[2, 4, 6]**
c