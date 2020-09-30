json - Javascript Object notation, which is the syntax for storing and exchanging data.

json in Python - JSON in built-in package and we can import, which can work with JSON data.
Syntax : 		import json

Convert from json to python - If we have json string and we want to convert json to python using json.loads() method
Eg:		import json
			x =  '{ "name":"John", "age":30, "city":"New York"}'# json string
			y = json.loads(x)# json to python conversation
			print(y["age"])# which display value as 30 	

Convert from json to python - if we have python objects and want to convert it into a json string using json.dumps() method
Eg:		import json
			#python object -dictionary
			x = {"name": "John", "age": 30, "city": "New York"} 
			y = json.dumps(x)#python to json conversation
			print(y)
			
We can convert the following python object into json string
dict 
Eg:		print(json.dumps({"name": "John", "age": 30}))
			# which returns{"name": "John", "age": 30}

list
Eg:		print(json.dumps(["apple", "bananas"]))
			# which returns ["apple", "bananas"]
	
tuple
Eg:		print(json.dumps(("apple", "bananas")))
			# which returns["apple", "bananas"]

string
Eg:		print(json.dumps("hello"))# which returns "hello"

int
Eg: 		print(json.dumps(42))# which returns 42 
				
float
Eg:		print(json.dumps(31.76))# which returns 31.76

True
Eg:		print(json.dumps(True))# which returns true

False
Eg:		print(json.dumps(False))# which returns false

None
 Eg:		print(json.dumps(None))# which returns null
	
Order the Result
If we want to sort the result alphabetically by keys, we can use sort_keys = True.
Eg:		import json
			x = {
		  "name": "John",
		  "age": 30,
		  "married": True,
		  "divorced": False,
		  "children": ("Ann","Billy"),
		  "pets": None,
		  "cars": [
	    {"model": "BMW 230", "mpg": 27.5},
	    {"model": "Ford Edge", "mpg": 24.1}
	  	]
		}
		print(json.dumps(x, sort_keys=True)) #sort the result alphabetically by keys

				
			
				
				
		