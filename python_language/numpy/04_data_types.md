# Data types that support Numpy

Below is a list of all data types in NumPy and the characters used to represent them.

| **Charecter** | **Data Types** |
|---------------|----------------|
|i  | integer |
|b  | boolean |
|u  |unsigned integer |
|f |float |
|c | complex float |
|m | timedelta |
|M | datetime |
|O | object |
|S | string |
|U | unicode string |
|V | fixed chunk of memory for other type ( void )|

* Checking Data Type of an array -  we can check the data type of objects in collections <br />
	*Eg*:	```import numpy as np``` <br />
			```arr = np.array([1, 2, 3, 4])``` <br />
			```print(arr.dtype)```
