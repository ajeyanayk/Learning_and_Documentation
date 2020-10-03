# json Module

**json - Javascript Object notation, which is the syntax for storing and exchanging data.**

* **json in Python** //JSON in built-in package and we can import, which can work with JSON data. <br />
	Syntax : ```import json```

**Convert from json to python** <br />
* If we have json string and we want to convert json to python using json.loads() method <br />
	*Eg*:	```import json``` <br />
			```x =  '{ "name":"John", "age":30, "city":"New York"}' ``` //json string <br />
			```y = json.loads(x)``` //json to python conversation <br />
			```print(y["age"])``` //which display value as 30 	

* If we have python objects and want to convert it into a json string using json.dumps() method <br />
	*Eg*:	```import json``` <br />
			//python object -dictionary <br />
			```x = {"name": "John", "age": 30, "city": "New York"}``` <br />
			```y = json.dumps(x)#python to json conversation``` <br />
			```print(y)```
			
####  We can convert the following python object into json string

**dict** <br />
	*Eg*:	```print(json.dumps({"name": "John", "age": 30}))``` //which returns{"name": "John", "age": 30} <br />

**list** <br />
	*Eg*:	```print(json.dumps(["apple", "bananas"]))``` //which returns ["apple", "bananas"] <br />
	
**tuple** <br />
	*Eg*:	```print(json.dumps(("apple", "bananas")))``` //which returns["apple", "bananas"] <br />

**string** <br />
	*Eg*:	```print(json.dumps("hello"))``` //which returns "hello" <br />

**int** <br />
	*Eg*: 	```print(json.dumps(42))``` //which returns 42  <br />
				
**float** <br />
	*Eg*:	```print(json.dumps(31.76))``` //which returns 31.76 <br />

**True** <br />
	*Eg*:	```print(json.dumps(True))``` //which returns true <br />

**False** <br />
	*Eg*:	```print(json.dumps(False))``` //which returns false <br />

**None** <br />
	*Eg*:	```print(json.dumps(None))``` //which returns null <br />
	
**Order the Result** <br />
* If we want to sort the result alphabetically by keys, we can use sort_keys = True. <br />
	*Eg*:	```import json``` <br />
			```x = {``` <br />
			```"name": "John",``` <br />
			```"age": 30,``` <br />
			```"married": True,``` <br />
			```"divorced": False,``` <br />
			```"children": ("Ann","Billy"),``` <br />
			```"pets": None,``` <br />
			```"cars": [``` <br />
			```{"model": "BMW 230", "mpg": 27.5},``` <br />
			```{"model": "Ford Edge", "mpg": 24.1}``` <br />
			```]``` <br />
			```}``` <br />
			```print(json.dumps(x, sort_keys=True))``` //sort the result alphabetically by keys

				
			
				
				
		