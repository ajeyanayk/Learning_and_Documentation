  <h1 align="center">If else loop</h1>

Python supports the following logical condition from mathematics

|Logical Condition | Description |
|------------------|----------|
| a == b | a Equals b |       
| a != b | a Not Equals b|
| a < b | a Less than b|
| a <= b | a Less than or equal to b |
| a > b | a Greater than b|
| a >= b | a Greater than or equal to b|

* if statement and loop starts with "if" and follows with condition or list of conditions and ends with colon(:) <br />
* All looping statements rely on indentation which means a wide space after each looping statement <br />

+ In *if statement* if the condition is true, then execute next following content or else it return with empty value <br />
	*Eg*:	
```python
			a = 33 
			b = 200 where a&b are variables 
			if b > a: 
 				 print("b is greater than a") start with indentation (a wide space) 
```

+ *Elif* - If the condition is not true, Instead of returning empty value , the loop will follow 	elif  statement and execute the content which it follows <br />
	*Eg*:		
```python
			a = 33 
			b = 33 
			if b > a: 
 				 print("b is greater than a") 
			elif a == b: 
  				print("a and b are equal") 
```

+ *Else* - if any of the condition is not true, then it execute else statement  and execute the content which it follows (we can have else statement without elif keyword too) <br />
	*Eg*:	
```python
			a = 200 
			b = 33 
			if b > a: 
 				 print("b is greater than a") 
			elif a == b: 
  				print("a and b are equal") 
			else: 
  				print("a is greater than b") 
```

* *Short Hand If* - If we have only one statement execute, we can put next line content in the same line <br />
	*Eg*:			
```python			
			a = 2 
			b = 330 
			if a > b: 
				print("a is greater than b") 
```

* *Short hand If... Else*

	+ If we only one statement for if and else, we can put in same line. If the condition is true then left side content will get execute, else it will execute right side content <br />
		*Eg*:	
	```python
				a = 2 
				b = 330 
				print("A") if a > b else print("B") 
	```
		
	+ If we have more than else system, we can put in same line. <br />
		*Eg*:	
	```python
			a = 330 
			b = 330 
			print("A") if a > b else print("=") if a == b else print("B") 
	```

+ *and* - and keyword is logical operator to combine two conditional statement (If both conditional Statements are true, it will execute the next content) <br />
	*Eg*: 	
```python
			a = 200 
			b = 33 
			c = 500 
			if a > b and c > a: 
  				print("Both conditions are True")
```

+ *or* - or keyword is logical operator to combine two conditional statement (If either of one conditional Statement is true, it will execute the next content) <br />
	*Eg*:	
```python
			a = 200 
			b = 33 
			c = 500 
			if a > b or a > c: 
  				print("At least one of the conditions is True")
```

+ **Nested If** - If we want to execute two if statement or if statement is under another if statement , we call it as nested if condition <br />
	*Eg*:	
```python			
			x = 41 
			if x > 10: 
  				print("Above ten,") 
			if x > 20: 
				print("and also above 20!") 
			else: 
				print("but not above 20.") 
```

+ **Pass** -  if in if statement, there is no content because of some reason and to avoid getting error message. we can type pass. <br />
	*Eg*:	
```python
			a = 33 
			b = 200 
			if b > a: 
				pass 
```