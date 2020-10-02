# Data Type

* If we want to check whether the object belongs to the certain datatype <br />
	Eg:	```x = "Ajeya Nayak"``` <br />
			```print(isinstance(x, str))``` <br />
			*which display shows True as x is string data type* 


#### The Types of data types in python

|Text Type:|str|
|-------|-------|
|Numeric Types |int, float, complex|
|Sequence Types |list, tuple, range|
|Mapping Type |dict|
|Set Types | set, frozenset|
|Boolean Type | bool |
|Binary Types |bytes, bytearray, memoryview|

* To find the data type of the variable, Type command <br />
	synatx ```print(type(variable_name))```
	
	
|Variable assigned as x   | Data Type|
|-----------------------|----------|
|x = "Hello World" | str |
|x = 20 | int |
|x = 20.5 |float |
|x = 1j | complex|
|x = ["apple", "banana", "cherry"]| list|
|x = ("apple", "banana", "cherry")| tuple|
|x = range(6) |range |
|x = {"name" : "John", "age" : 36} | dict |
|x = {"apple", "banana", "cherry"} | set |
|x = frozenset({"apple", "banana", "cherry"}) |frozenset|
|x = True | bool|
|x = b"Hello" | bytes |
|x = bytearray(5)| bytearray|
|x = memoryview(bytes(5)) | memoryview|
