# Module 

**Module is like a code Library, from which another file will take set of function for perform tasks.**

* **Create a Module** - to create a module need to save with script  which we are using in future purpose and save it with extension .py <br />
	*Eg*:	```def greeting(name):``` <br />
			  ```print("Hello, " + name)``` <br />
			//save this script with mymodule.py

* **Use a Module** -   with the reference from mymodule.py, we need to create a file with script and mention file name from where we imported. <br />
	*Eg*:	```import mymodule``` <br />
<br />		``` ```
			```mymodule.greeting("Jonathan")``` //we are using greeting function from mymodule.py <br />

* **Variables in Module** - the module may have functions, variables like, list,dictionary or object. <br />
	*Eg*:	```person1 = {"name": "John",  "age": 36,  "country": "Norway"}``` //save file as mymoudle.py <br />
 <br />		``` ```
			//open newfile <br />
			```import mymodule``` <br />
			```a = mymodule.person1["age"]``` //module_file_name.function_name["Key"] <br />
			//used "key" because variable is dictionary <br />
			```print(a)```

**Naming & Renaming Module**

* We can save the module with any name, But it should end with .py <br />
* We can rename the module when we are importing <br />
	*Eg*:	```import mymodule as mx # mymodule renamed to mx``` <br />
			```a = mx.person1["age"]``` <br />
			```print(a)```

**Built-in Modules** //There are several built-in modules which we can import when we are required. <br />
	*Eg*:	```import platform``` //module platform <br />
			```x = platform.system()``` //System is function <br />
			```print(x)```

**Using the dir() Function** //dir() function to find function names ,variables. <br />
	*Eg*:	```import platform``` <br />
			```x = dir(platform)``` //which displays all variables and function in this module <br />
			```print(x)```	

**Import from Module** <br />
* we can import a part or function from Module by using from keyword. <br />
	*Eg*:  //creating file (module) as mymodule.py <br />
			```def greeting(name):``` <br />
			  ```print("Hello, " + name)``` <br />
<br />		``` ```
			```person1 = {"name": "John", "age": 36, "country": "Norway"}``` <br />
<br />		``` ```			
			//import function or variables from module in another file <br />
			```from mymodule import person1``` // mymodule is module and person is variable <br />
		`	```print (person1["age"]) # no need to mention module name again```

		