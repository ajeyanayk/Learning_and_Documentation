# Function in Python

**Function is set of code which runs only if it is called and it returns with data as a result** <br />

* **Creating function** - function is defined with def keyword <br />
	*Eg*:	```def my_function():``` <br />
  			```print("Hello from a function")``` *Indentation* 

* **Calling function** - we can call the function by using function name with parenthesis <br />
	*Eg*:	```def my_function():``` <br />
  			```print("Hello from a function")``` <br />
<br />		``` ```
			```my_function()```

**Arguments** <br />

+ Information can be passed through into function as arguments  <br />
+ Arguments are specified after the function name with closed parenthesis 

* We can pass "n" number of arguments while calling function and it should be separated by coma(,). <br />
	*Eg*:	```def my_function(fname):``` *specifying argument* <br />
  			```print(fname + " Refsnes")```  <br />
<br />		``` ```
			```my_function("Emil")```  *passing argument* <br /> 
			```my_function("Tobias")```  <br />
			```my_function("Linus")``` 

* By default, The number of arguments are depending on number of arguments mentioned defined in function, nothing more or nothing less. <br />
	*Eg*:	```def my_function(fname, lname):``` *2 arguments are mentioned* <br />
  			```print(fname + " " + lname)``` <br />
<br />		``` ```
			```my_function("Emil", "Refsnes")``` *2 arguments are passed*

**Arbitrary Arguments,** ***args** <br />
* If we don't know how many arguments that will be passed through function, we need to mention with * and then write argument name. <br />
	*Eg*:	```def my_function(*kids):```  *argument kids start with ** <br />
			  ```print("The youngest child is " + kids[2])``` <br />
		*which displays "The youngest child is Linus as it is" index 2* <br />
			```my_function("Emil", "Tobias", "Linus" )```

**Keyword Arguments** <br />
* If we want send the argument with key = value Syntax <br />
	*Eg*:	```def my_function(child3, child2, child1):```  <br />
 				```print("The youngest child is " + child3)``` <br />
			```my_function(child1 = "Emil", child2 = "Tobias", child3 = "Linus")``` <br />
			*the order of the arguments does not matter*

**Arbitrary Keyword Arguments,** ****kwargs,** <br />
* If we don't know how many argument with key = value syntax, we need to mention with ** <br />
	*Eg*;	```def my_function(**kid):``` <br />
			  ```print("His last name is " + kid["lname"])``` # displays His last name is Refsnes <br />
<br />			``` ```
			```my_function(fname = "Tobias", lname = "Refsnes")```

**Default Parameter Value** <br />
* If we are calling the function without argument , it uses the default value <br />
	*Eg*:	```def my_function(country = "Norway"):```*Default argument is country = "Norway"* <br />
			  ```print("I am from " + country)``` <br />
<br />			``` ```
			```my_function("Sweden")``` <br />
			```my_function("India")``` <br />
			```my_function()``` <br />
			```my_function("Brazil")``` <br />
			*which displays output as* <br />
				**I am from Sweden** <br />
				**I am from India** <br />
				**I am from Norway** <br />
				**I am from Brazil**

**Passing Lists as an argument** <br />
* If we want to pass argument from Lists to function  <br />
	*Eg*:	```def my_function(food):``` <br />
			  ```for x in food:``` <br />
			    ```print(x)``` *which displays apple, banana, cherry* <br />
<br />		``` ```
			```fruits = ["apple", "banana", "cherry"]```  <br />
			```my_function(fruits)``` 

**Return Values** <br />
* If we want to return value where we called the function <br />
	*Eg*:	```def my_function(x):``` <br />
 				```return 5 * x``` *take value from function and return value once exp is executed* <br />
<br />		``` ```
			```print(my_function(3))``` *send arg to function and display the value once returned* <br />
			```print(my_function(5))``` <br />
			```print(my_function(9))``` 

**Pass Statement** <br />
* If the function is defined, But it doesn't any content because of some reason. Instead of getting error message we need to put pass <br />
	**Eg**:	```def myfunction():``` <br />
 			 ```pass``` 

**Recursion** - If the function call itself  

**Recursion is a common mathematical and programming concept. It means that a function calls itself. This has the benefit of meaning that you can loop through data to reach a result.** <br />
	*Eg*:	```def tri_recursion(k):``` <br />
  				```if(k > 0):``` <br />
   				 	```result = k + tri_recursion(k - 1)``` <br />
			    	```print(result)``` <br />
			  	```else:``` <br />
			    	```result = 0``` <br />
					```return result``` <br />
<br />		``` ```
			```print("\n\nRecursion Example Results")``` <br />
<br />		``` ```
			```tri_recursion(6)``` <br />
<br />		``` ```
			*which displays* <br />
			**Recursion Example Results** <br />
					**1** <br />
					**3** <br />
					**6** <br />
					**10** <br />
					**15** <br />
					**21**






			



 