 Module is like a code Library, from which another file will take set of function for perform tasks.

Create a Module - to create a module need to save with script  which we are using in future purpose and save it with extension .py
Eg:		def greeting(name):x
			  print("Hello, " + name)
			# save this script with mymodule.py

Use a Module -   with the reference from mymodule.py, we need to create a file with script and mention file name from where we imported.
Eg:		import mymodule
			mymodule.greeting("Jonathan") #we are using greeting function from mymodule.py

Variables in Module - the module may have functions, variables like, list,dictionary or object.
Eg:	person1 = {"name": "John",  "age": 36,  "country": "Norway"}# save file as mymoudle.py
		
		#open newfile
		import mymodule
		a = mymodule.person1["age"] # module_file_name.function_name["Key"] 
		# i used "key" because variable is dictionary
		print(a)

Naming & Renaming Module
We can save the module with any name, But it should end with .py
We can rename the module when we are importing
Eg:			import mymodule as mx # mymodule renamed to mx
				a = mx.person1["age"]
				print(a)

Built-in Modules - There are several built-in modules which we can import when we are required.
Eg:	import platform # module platform
		x = platform.system() # System is function
		print(x)

Using the dir() Function - dir() function to find function names ,variables.
Eg:		import platform
			x = dir(platform) # which displays all variables and function in this module
			print(x)		

Import from Module
	we can import a part or function from Module by using from keyword.
Eg: 		# creating file (module) as mymodule.py
			def greeting(name):
			  print("Hello, " + name)

			person1 = {"name": "John", "age": 36, "country": "Norway"}
			
			#import function or variables from module in another file
			from mymodule import person1 # mymodule is module and person is variable
		`	print (person1["age"]) # no need to mention module name again

		