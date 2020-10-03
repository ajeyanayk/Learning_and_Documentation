# For loop

**for loop is used for iterating over sequence (that is either a list, a tuple, a dictionary, a set, or a string).** <br />
	*Eg*:	```fruits = ["apple", "banana", "cherry"]``` <br />
			```for x in fruits:``` <br />
  					```print(x)``` <br />
			*which displays fruits name in order like* <br />
						**apple** <br />
						**banana** <br />
						**cherry**

* If the object is string, then it display individual character <br />
	*Eg*:	```for x in "banana":``` <br />
 				```print(x)``` <br />
			*which displays fruits name in order like* <br />
						**b** <br />
						**a** <br />
						**n** <br />
						**a** <br />
						**n** <br />
						**a**

* **Break Statement** - like in while loop, we can stop the loop even though statement is true using break statement <br />
	*Eg*:	```fruits = ["apple", "banana", "cherry"]``` <br />
			```for x in fruits:``` <br />
			  	```print(x)``` <br />
			```if x == "banana":``` <br />
			    ```break```  <br />
			*which displays fruits name in order like* <br />
					**apple** <br />
					**banana** 

* **continue statement** - like in while loo, we can stop current iteration and continue next <br />
	*Eg*:	```fruits = ["apple", "banana", "cherry"]``` <br />
			```for x in fruits:``` <br />
			  ```if x == "banana":``` <br />
			    	```continue``` <br />
			 		```print(x)``` <br />
			*which displays fruits name in order like* <br />
					**apple** <br />
					**cherry** 

**range function** <br />

* we can set range to specified number of time the set of sequence to be repeated , as  default which starts with 0 , and increment of 1, and end at specified number <br />
	*Eg*:	```for x in range(6):``` <br />
  				```print(x)``` *which prints 0,1,2,3,4 & 5* 

* we can set range to specified number of time the set of sequence to be repeated and we can set start and end range with increment of 1. <br />
	*Eg*:	```for x in range(2, 6):``` <br />
  				```print(x)``` *which displays 2,3,4 & 5* 

* If we want to specify the increment  range <br />
	*Eg*:	```for x in range(2, 30, 3):``` <br />
  				```print(x)``` *which prints 2,5,8,11,14,17,20,23,26 &29.*
 		
* else in for loop  - like in if statement and for loop,we can use else statement if the for loop condition is false <br />
	*Eg*:	```for x in range(6):``` <br />
  				```print(x)``` <br />
			```else:``` <br />
				```print("Finally finished!")``` <br />
				*which displays* <br />
					**0** <br />
					**1** <br />
					**2** <br />
					**3** <br />
					**4** <br />
					**5** <br />
				*Finally finished!*

* **Nested If*** - If we want to execute two for loop statement or for loop statement is under another for loop statement,The "inner loop" will be executed one time for each iteration of the "outer loop" <br />
	*Eg*:	```adj = ["red", "big", "tasty"]``` <br />
			```fruits = ["apple", "banana", "cherry"]``` <br />
			```for x in adj:``` <br />
			  	```for y in fruits:``` <br />
			    		```print(x, y)``` <br />
				*which prints* <br />
				  **red apple** <br />
				  **red banana** <br />
				  **red cherry** <br />
				  **big apple** <br />
				  **big banana** <br />
				  **big cherry** <br />
				  **tasty apple** <br />
				  **tasty banana** <br />
				  **tasty cherry**

* **Pass** -  like in if statement, if there is no content in for loop statement because of some reason and to avoid getting error message. we can type pass. <br />
	*Eg*: 	```for x in [0, 1, 2]:``` <br />
				  ```pass```

	*Eg*:	```a = 33``` <br />
			```b = 200``` <br />
			```if b > a:``` <br />
				```pass```