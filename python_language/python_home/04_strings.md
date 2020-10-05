<h1 align="center">Python String</h1>

*String are surrounded by double quotation or single quotation mark* <br />
	*Eg*: `"Ajey"  or 'Ramanath'`

* If we want to display string ```print("Ajey")``` or ```print('Ramanath')``` <br />

<ins>**Assigning the string value to variable**</ins>

* If we want to assign single line string to variable then we need to use single or double quotation marks after and before the string. <br />
		*Eg*: `a = "Ajey Nayak"`

* If we want to assign multi line string to variable then we need to use three double quotation mark(""") or single quotation mark(''') <br />
		*Eg*: `x = """My name is Ajey``<br />
						`I am learning python since 2 months`<br />
						`I want to be come a successful Python - developer"""`<br />

<ins>**Python does not have character data type**</ins>

+ String are Arrays - If we want to access a element of the string the we can the index method inside the square bracket <br />
		*Eg*:  
```python
		a = "Hello"
		print(a[1]) //which display the character "e" as the string element start with index 0.
```

+ *Slicing* - If we want to access a set of element of the string. <br />
		*Eg*:  
```python
		b = "Unglaublisch"
		print(b[2:7]) //which the element "glaub" (from index 2 to 7
```

+ Negative Indexing** - if we want access last few elements of the string. <br />
		*Eg*:  
```python
		c= "Meinung"
		print(c[-6:-1] //which displays "einung" (from index -5 to -1)
```

+ *String Length* - If we want to find the length of the string, we can use **len()**  <br />
		*Eg*: 
```python
		d= "Ajeya Nayak"
		print(len(d)) //which displays 11
```		

<ins>**String Methods:**</ins>

+ *strip()* - which removes the space from begging or the end and which will not remove the space between two words. <br />
		*Eg*: 	
```python
		a = "Computer System" 
		print(a.strip())  //which shows as *Computer System*
```
			  
+ *lower()* - which converts the string to lower case <br />
		*Eg*:  
```python
		a="Computer System" 
		print(a.lower())  //which shows as *computer system*
```
			   
+ *upper()* - which converts the string to upper case <br />
		*Eg*: 
```python
		a="Computer System" 
		print(a.upper()) //which shows as *COMPUTER SYSTEM*
```

+ *replace* - which replace the character from one to another. and which is case sensitive <br />
		*Eg*:  
```python
		b ="bellphone" 
		print(b.replace("b","c")  //which shows as *cellphone*
```
			   
+ *split* - which divides the string in two or more sub-string , if there is instances separator. <br /> 
		*Eg*:  
```python
		c="Ajeya Nayak" 
		print(c.split(" "))  //which split into two sub-string with separator "," at last it shows ['Ajeya' , 'Nayak']
```

* check String - If we want to check the certain phrase or character present or not, We can use the keyword "in"  for present and "not in" for absent cases. <br />
	+ For "in" cases <br />
	```python
			txt = "My town is karkala" 
			x =  "karkala" in txt 
			print(x) //which displays *True*
			y= "city" in txt 
			print(y)  //which displays *False*
	``` 

	+ For "not in" cases <br />
	```python
			cnt = "Electricity" 
			a = "town" not in cnt 
			print(a) //which shows *True *
			b = "ect" not in cnt 
			print(b) //which shows *False*
	```

* String Concatenation we need to use + operator for merge two strings and this method will not support a string and an Integer <br />
	*Eg*:
```python
		a= "Uttar" 
		b= " Pradesh" 
		print(a + b) //which display value as "Uttar Pradesh"
```		

* String Format

	+ If we want to combine string and integer, Then we need to use *format()* method to concatenate. <br />
		*Eg*:	
	```python
			state = 31 
			txt = "There are {} states in India" 
			print(txt.format(state)) //which display as "There are 31 states in India"
	```

	+ If there are more than one Integer, <br />
		*Eg*:
	```python
			sta = 31 
			cap = 3 
			con=7 
			txt="World has {} continent , There are {} states in India and Andhra Pradesh has {} capitals." 
			print(txt.format(con,sta,cap)) 
			//which dispaly as World has 7 continent , There are 31 states in India and Andhra Pradesh has 3 capitals.
	```

* Escape Character

	+ If we want to insert special character  which are illegal in string i.e, "", backspace or Newline, Then we need to use \ before inserting special character <br />
		*Eg*: `print("India\'s capital is New Delhi")` //which displays output as *India's capital is New Delhi*