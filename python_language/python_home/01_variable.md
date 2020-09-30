Variable - Which are containers for storing data values.

Rules for variable
A variable name must start with a letter or the underscore character
A variable name cannot start with a number
A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
Variable names are case-sensitive (age, Age and AGE are three different variables)

#Legal variable names:										#Illegal variable names:
	myvar = "John"												2myvar = "John"
	my_var = "John"											my-var = "John
    _my_var = "John"
	myVar = "John"
	MYVAR = "John"
	myvar2 = "John"

Assign the values to multiple variable
Eg: x,y,z = " Orange", "White", "Green"

 Assigning same values to multiple variable
Eg:  x = y = z =  "Blue"

If we create a variable with the same name inside a function, this variable will be local, and can only be used inside the function. The global variable with the same name will remain as it was, global and with the original value.
Eg:
		x = "awesome"

		def myfunc():
		  x = "fantastic"
  print("Python is " + x) # output is Python is fantastic
myfunc()

print("Python is " + x) # output is Python is awesome

If we use the global keyword , the variable can use inside as well out side
	Eg:
			x = "awesome"

			def myfunc():
  			global x
  			x = "fantastic"
			print("Python is " + x) # out put - Python is fantastic
			myfunc()

			print("Python is " + x) # out put - Python is fantastic