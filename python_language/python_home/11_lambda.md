# Lambda Function

**lambda function is small function, which takes any number of arguments, but can only have one expression and return with result** <br />
	Syntax: ```lambda arguments : expression``` <br />
<br />		``` ```
	*Eg*:	```x = lambda a : a + 10``` * it took an argument and return the value* <br />
			```print(x(5))``` *which displays value 15* <br />
<br />		``` ```	
			```y = lambda a, b : a * b``` *it took 2 arguments and return the value* <br />
			```print(x(5, 6))``` *which display as 30* 

* we can use lambda inside function,which will take the argument without creating function. <br />
	Syntax:	```def myfunc(n):``` <br />
  				```return lambda a : a * n``` 

	*Eg*: 	```def myfunc(n):``` <br />
			  ```return lambda a : a * n```  *lambda is acting here as function mydoubler* <br />
<br />		``` ```
			```mydoubler = myfunc(2)``` <br />
			```print(mydoubler(11))``` *which will pass the argument to lambda function* 

* We can execute multiple expression with one lambda function <br />

	*Eg*:	```def myfunc(n): <br />
			  ```return lambda a : a * n <br />
<br />		``` ```
			```mydoubler = myfunc(2)``` *which is expression 1* <br />
			```mytripler = myfunc(3)``` *which is expression 1* <br />
<br />		``` ```
			```print(mydoubler(11))```  <br />
			```print(mytripler(11))```  <br />









