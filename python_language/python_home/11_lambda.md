<h1 align="center">Lambda Function</h1>

lambda function is small function, which takes any number of arguments, but can only have one expression and return with result <br />
	Syntax: `lambda arguments : expression` <br />
	*Eg*:	
```python
			x = lambda a : a + 10 //it took an argument and return the value
			print(x(5)) //which displays value 15
		 	
			y = lambda a, b : a * b //it took 2 arguments and return the value 
			print(x(5, 6)) //which display as 30
```

* we can use lambda inside function,which will take the argument without creating function. <br />
	Syntax:	
```python
			def myfunc(n):
  				return lambda a : a * n
```
	 Eg: 	
  ```python
		  def myfunc(n): 
			    return lambda a : a * n  //lambda is acting here as function mydoubler
		 
			mydoubler = myfunc(2) 
			print(mydoubler(11))  //which will pass the argument to lambda function
```

* We can execute multiple expression with one lambda function <br />
	*Eg*:	
```python
		def myfunc(n): 
			  return lambda a : a * n 
		 
		mydoubler = myfunc(2)  //which is expression 1* 
		mytripler = myfunc(3)  //which is expression 1* 
		 
		print(mydoubler(11))  
		print(mytripler(11))  
```









