<h1 align="center">Math Module</h1>

To perform Mathematical tasks on numbers, we can import math module

**Built-in Math Functions**

| **Math Function** | **Description** |
|---------------|-----------------|
| min() | to return the lowest value in an iterable |
| max() | to return the  lowest value in an iterable |
| abs() | to return the absolute(positive) value of specified number. |
| pow(x,y) | to return the value of x the power of y |

*Eg*: 	
```python
		w = min(5, 10, 25) 
		x = max(5, 10, 25) 
		y = abs(-7.25) 
		x = pow(4, 3) 
	 
		print(w) //which returns the value 5  
		print(x) //which returns the value 25 
		print(y) //which returns the value 7.25 
		print(z) //which returns the value 64
```

* *math.sqrt()* - this function returns the square root of the mentioned number inside the square bracket. <br />
	*Eg*:	
```python
		import math 
		x = math.sqrt(64) 
		print(x) // which returns the value 8
```

* *math.ceil()*- method rounds a number upwards to its nearest integer. <br />
* *math.floor()*- method rounds a number downwards to its nearest integer. <br />
* *math.pi()*- function return the pei value. <br />
	*Eg*:	
```python
		import math 
		x = math.ceil(1.4) 
		y = math.floor(1.4) 
		z = math.pi 
		print(x) //returns 2 
		print(y) //returns 1 
		print(z) //returns 3.14...
```