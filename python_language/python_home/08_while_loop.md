# While loop

+ In while loop, we can execute the set of statement till the condition is True <br />
	*Eg*:	```i = 1``` <br />
			```while i < 6:``` <br />
  				```print(i)``` *which execute the number from 1 to 5* <br />
  				```i += 1```

+ **The break statement** - in this statement we can stop the loop even though the statement is True.  <br />
	*Eg*:	```i = 1``` <br />
			```while i < 6:``` <br />
				```print(i)``` <br />
			```if i == 3:``` <br />
		    	```break``` <br />
			```i += 1``` *which displays only 1 ,2 & 3* 

+ **The continue statement** -  in this statement , we can stop the iteration and continue with next statement <br />
	*Eg*:	```i = 0``` <br />
			```while i < 6:``` <br />
				```i += 1``` <br />
			```if i == 3:``` <br />
				```continue``` <br />
			  ```print(i)``` *which displays only 1 ,2,4,5 & 6*

+ **else statement** - like if statement, we can use else statement if while condition is False <br />
	*Eg*:		```i = 1``` <br />
				```while i < 6:``` <br />
  					```print(i)``` <br />
  					```i += 1``` <br />
				```else:``` <br />
	 				```print("i is no longer less than 6")``` <br />