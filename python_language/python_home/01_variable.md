<h1 align="center">Python Variable</h1>

Variable - Which are containers for storing data values.

* Rules for variable <br />
	+ A variable name must start with a letter or the underscore character <br />
	+ A variable name cannot start with a number <br />
	+ A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )<br />
	+ Variable names are case-sensitive (age, Age and AGE are three different variables) 

* Legal variable names <br />

	myvar = "John" <br />										
	my_var = "John" <br />									
	_my_var = "John" <br />
	myVar = "John" <br />
	MYVAR = "John" <br />
	myvar2 = "John"`] 

* Illegal variable names <br />
	my-var = "John" <br />
	2myvar = "John" 

* Assign the values to multiple variable <br />
	*Eg*: `x,y,z = " Orange", "White", "Green"`

* Assigning same values to multiple variable <br />
	*Eg*: `x = y = z =  "Blue"`

* If we create a variable with the same name inside a function, this variable will be local, and can only be used inside the function. The global variable with the same name will remain as it was, global and with the original value. <br />
	*Eg*: 
```python
	x = "awesome"
	def myfunc():
		x = "fantastic"
  		print("Python is " + x) //output is Python is **fantastic**
	
	myfunc()
	print("Python is " + x) //output is Python is **awesome** 
```

* If we use the global keyword , the variable can use inside as well out side <br />
	*Eg*:	
```python	
	x = "awesome"
	def myfunc():
		global x
		x = "fantastic"
	print("Python is " + x) //output - Python is* **fantastic**
	
		myfunc()
	print("Python is " + x) //output is Python is **awesome** 
```