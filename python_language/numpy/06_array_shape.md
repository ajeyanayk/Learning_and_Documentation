# Array Shape

* Array shape , which means the number element in each dimension and we can find by using **shape()** method. <br />
	*Eg  1*:	```import numpy as np``` <br />
				```arr = np.array([[1, 2, 3, 4], [5, 6, 7, 8]])``` <br />
				```print(arr.shape)``` *returns (2,4), here 2 is dimension and 4 is elements in each dim.*

	*Eg 2*:		```import numpy as np``` <br />
				 *creating an array with 6 dimension* <br />
				```arr = np.array(([[1, 2, 3, 4], [5, 6, 7, 8]]), ndmin=6)``` <br />
				```print(arr)``` <br />
				*which displays* <br />
				```[[[[[[1 2 3 4] <br />
						[5 6 7 8]]]]]]``` <br />
				```print('shape of array :', arr.shape)``` <br />
				*returns shape of array :* **(1, 1, 1, 1, 2, 4)**
				


 