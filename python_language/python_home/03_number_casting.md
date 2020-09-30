There are 3 numeric types in Python - int, float & complex
Int - Int, or integer, is a whole number, positive or negative, without decimals, of unlimited length.
			Eg:  	x = 100
					y = -15242
					z = -852643

Float - Float, or "floating point number" is a number, positive or negative, containing one or scientific numbers with an "e" to indicate the power of 10.
			Eg:  	w = 0.205
					x  = -1524.526
					y  =  125e2
					z  = 125.256e25

Complex - complex numbers with an imaginary part "j"
			Eg:   x = 256.3+2j
					y = 152j
					z = -489j

Type conversion

if we want to convert one data type to another data type 
Eg:
a = 1
b = 25.6

x = float(a) # float()- to covert integer to float
y = int(b)   # int()- to covert float to integer
z = complex(b) # complex() - to convert integer/float values to complex

print(type(x)) # output - <class 'float'>
print(type(y)) # output - <class 'integer'>
print(type(z)) # output - <class 'complex'>

 Please note we cant convert complex values to integer or float.

# if we want to select random number in the range of numbers
import random

print(random.randrange(1, 1000)  # displays random numbers between 1 to 1000



Casting : If we want to change the data type the variable, we can use the constructor function.
int(), this function will change the data type from float to integer, we can not change the string value to integer.
	Eg: 	x = int(10.05)
			print(x) # which display the value as 10

float(), this function will change the data type from integer to float, we can not change the string value to float.
	Eg: 	y= float(15)
			print(y) # which display the value as 15.0

str(), this function will change the value to string values, Integer literals or float literals
	Eg:   x= str(10)
	  		y=str(16.3)
			print(x), # which display as "10" and which is not integer.
			print(y), # which display as "16.3" and which is not float value