# Exception Handling (try.. except)

* When an error occurs or exception and we want to stop and generate an error messages <br />
* We have three keywords to block and generate an error message

+ **try** - which blocks and generate an exception <br />
+ **except** -  which blocks and handle error <br />
+ **finally**	-  it allows  execute the code irrespective of try or except blocks.

**Exception Handling** <br />
	*Eg*: 	```try:``` <br />
 		 		```print(x)``` //try will generate an exception as x is not defined <br />
			```except:``` <br />
 		 		```print("An exception occurred")``` //exception blocks and show error message if mentioned.

**Many Exception <br />
* we can generate many exception blocks as we want. <br />
	*Eg*:	```try:``` <br />
			  	```print(x)``` <br />
			```except NameError:```  <br />
			  	```print("Variable x is not defined")``` <br />
			```except:``` <br />
			  	```print("Something else went wrong")```

* **Else** - we can use the else keyword , if there is no error were raised. <br />
	*Eg*:	```try:``` <br />
 			 	```print("Hello")``` <br />
			```except:``` <br />
			  	```print("Something went wrong")``` <br />
			```else:``` <br />
			  	```print("Nothing went wrong")```

* **finally** - If finally block specified, will be executed whether try or except will raise an error or not <br />
	*Eg 1* : ```try:``` <br />
			  	```print(x)``` //try will generate an exception as x is not defined <br />
			```except:``` <br />
			  	```print("Something went wrong")``` <br />
			//As exception created will generate an error message  <br />
			```finally:``` <br />
			  	```print("The 'try except' is finished")```

	*Eg 2* : ```try:``` <br />
				  ```f = open("demofile.txt")``` <br />
				  ```f.write("Lorum Ipsum")``` <br />
			 ```except:``` <br />
				  ```print("Something went wrong when writing to the file")``` <br />
			 ```finally:``` <br />
				  ```f.close()```

* **Raise an exception** <br />
* if any error occurs during any condition, we can raise an exception by throwing an error. <br />
	*Eg 1* :	```x = -1``` <br />
				```if x < 0:``` <br />
			  		```raise Exception("Sorry, no numbers below zero")```



