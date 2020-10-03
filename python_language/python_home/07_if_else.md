# If else loop

#### Python supports the following logical condition from mathematics

|Logical Condition | Description |
|------------------|-------------------------------|
| a == b| a Equals b |       
| a != b| a Not Equals b|
| a < b | a Less than b|
| a <= b| a Less than or equal to b |
| a > b | a Greater than b|
| a >= b | a Greater than or equal to b|

* if statement and loop starts with "if" and follows with condition or list of conditions and ends with colon(:) <br />
* All looping statements rely on indentation which means a wide space after each looping statement <br />

+ In **if statement** if the condition is true, then execute next following content or else it return with empty value <br /> 

	*Eg*:	```a = 33``` <br />
			```b = 200``` *where a&b are variables* <br />
			```if b > a:``` <br />
 				 ```print("b is greater than a")``` *start with indentation (a wide space)* <br />

+ **Elif** - If the condition is not true, Instead of returning empty value , the loop will follow 	elif  statement and execute the content which it follows <br />
	*Eg*:	```a = 33``` <br />
			```b = 33``` <br />
			```if b > a:``` <br />
 				 ```print("b is greater than a")``` <br />
			```elif a == b:``` <br />
  				```print("a and b are equal")``` <br />

+ **Else** - if any of the condition is not true, then it execute else statement  and execute the content which it follows (we can have else statement without elif keyword too) <br />
	*Eg*:	```a = 200``` <br />
			```b = 33``` <br />
			```if b > a:``` <br />
 				 ```print("b is greater than a")``` <br />
			```elif a == b:``` <br />
  				```print("a and b are equal")``` <br />
			```else:``` <br />
  				```print("a is greater than b")``` <br />

**Short Hand If**
		
+ If we have only one statement execute, we can put next line content in the same line <br />
	*Eg*:	```a = 2``` <br />
			```b = 330``` <br />
			```if a > b:``` <br />
				```print("a is greater than b")``` <br />

**Short hand If... Else** 

+ If we only one statement for if and else, we can put in same line. If the condition is true then left side content will get execute, else it will execute right side content <br />
	*Eg*:	```a = 2``` <br />
			```b = 330``` <br />
			```print("A") if a > b else print("B")``` <br />
		
+ if we have more than else system, we can put in same line. <br />
	*Eg*:	```a = 330``` <br />
			```b = 330``` <br />
			```print("A") if a > b else print("=") if a == b else print("B")``` <br />

+ **and** - and keyword is logical operator to combine two conditional statement (If both conditional Statements are true, it will execute the next content) <br />
	*Eg*: 	```a = 200``` <br />
			```b = 33``` <br />
			```c = 500``` <br />
			```if a > b and c > a:``` <br />
  				```print("Both conditions are True")```

+ **or** -  or keyword is logical operator to combine two conditional statement (If either of one conditional Statement is true, it will execute the next content) <br />
	*Eg*:	```a = 200``` <br />
			```b = 33``` <br />
			```c = 500``` <br />
			```if a > b or a > c:``` <br />
  				```print("At least one of the conditions is True")```

+ **Nested If** - If we want to execute two if statement or if statement is under another if statement , we call it as nested if condition <br />
	*Eg*:	```x = 41``` <br />
			```if x > 10:``` <br />
  				```print("Above ten,")``` <br />
			```if x > 20:``` <br />
				```print("and also above 20!")``` <br />
			```else:``` <br />
				```print("but not above 20.")``` <br />

+ **Pass** -  if in if statement, there is no content because of some reason and to avoid getting error message. we can type pass. <br />
	*Eg*:	```a = 33``` <br />
			```b = 200``` <br />
			```if b > a:``` <br />
				```pass``` <br />