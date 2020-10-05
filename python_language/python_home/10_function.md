<h1 align="center">Function in Python</h1>

Function is set of code which runs only if it is called and it returns with data as a result

* *Creating function* - function is defined with def keyword <br />
	*Eg*:	
```python
			def my_function():
  				print("Hello from a function") //Indentation
```

* *Calling function* - we can call the function by using function name with parenthesis <br />
	*Eg*:	
```python
		def my_function(): 
  			print("Hello from a function") 
		 
		my_function() //calling function
```

<ins>**Arguments**</ins>

+ Information can be passed through into function as arguments  <br />
+ Arguments are specified after the function name with closed parenthesis 

* We can pass "n" number of arguments while calling function and it should be separated by coma(,). <br />
	*Eg*:	
```python
		def my_function(fname): //specifying argument
  			print(fname + " Refsnes")  
		 
			my_function("Emil") //passing argument
			my_function("Tobias")  
			my_function("Linus") 
```
* By default, The number of arguments are depending on number of arguments mentioned defined in function, nothing more or nothing less. <br />
	*Eg*:	
```python
		def my_function(fname, lname): //2 arguments are mentioned* 
  			print(fname + " " + lname) 
		 
			my_function("Emil", "Refsnes") //2 arguments are passed*
```

*Arbitrary Arguments,* *\*args* <br />
* If we don't know how many arguments that will be passed through function, we need to mention with * and then write argument name. <br />
	*Eg*:	
```python
		def my_function(*kids):  *argument kids start with ** 
			  print("The youngest child is " + kids[2]) 
		//which displays "The youngest child is Linus as it is" index 2 
			my_function("Emil", "Tobias", "Linus" )
```

* *Keyword Arguments* <br />
* If we want send the argument with key = value Syntax <br />
	*Eg*:	
```python
			def my_function(child3, child2, child1):  
 				print("The youngest child is " + child3) 

			my_function(child1 = "Emil", child2 = "Tobias", child3 = "Linus") 
			//the order of the arguments does not matter
```
* *Arbitrary Keyword Arguments,* \*\*kwargs, If we don't know how many argument with key = value syntax, we need to mention with \* and then write argument name. <br />
	*Eg*;	
```python
		def my_function(**kid): 
			  print("His last name is " + kid["lname"]) //displays His last name is Refsnes 
			 
			my_function(fname = "Tobias", lname = "Refsnes")
```

* *Default Parameter Value* - If we are calling the function without argument , it uses the default value <br />
	*Eg*:	
```python
		def my_function(country = "Norway"): //Default argument is country = "Norway"* 
			  print("I am from " + country) 
			 
			my_function("Sweden") 
			my_function("India") 
			my_function() 
			my_function("Brazil") 
			//which displays output as
				I am from Sweden 
				I am from India 
				I am from Norway 
				I am from Brazil
```

* *Passing Lists as an argument* - If we want to pass argument from Lists to function  <br />
	*Eg*:	
```python
		def my_function(food): 
			  for x in food: 
			    print(x) *which displays apple, banana, cherry* 
		 
			fruits = ["apple", "banana", "cherry"]  
			my_function(fruits) 
```

* *Return Values* - If we want to return value where we called the function <br />
	*Eg*:	
```python
			def my_function(x): 
 				return 5 * x  //take value from function and return value once exp is executed 
		 
			print(my_function(3))  //send arg to function and display the value once returned
			print(my_function(5)) 
			print(my_function(9)) 
```

* *Pass Statement* - If the function is defined, But it doesn't any content because of some reason. Instead of getting error message we need to put pass <br />
	**Eg**:	
```python
			def my_function(x): 
 			 	pass
```

* Recursion* - If the function call itself and common mathematical and programming concept. It means that a function calls itself. This has the benefit of meaning that you can loop through data to reach a result. <br />
	*Eg*:	
```python
			def tri_recursion(k): 
  				if(k > 0): 
   				 	result = k + tri_recursion(k - 1) 
			    	print(result) 
			  	else: 
			    	result = 0 
					return result 
		 
			print("\n\nRecursion Example Results") 
		 
			tri_recursion(6) 
		 
			//which displays* 
			Recursion Example Results 
					1 
					3 
					6 
					10 
					15 
					21
```




			



 