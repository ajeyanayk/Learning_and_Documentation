# Python String

**String are surrounded by double quotation or single quotation mark** <br />
	*Eg*: ```"Ajey"  or 'Ramanath'```

* If we want to display string ```print("Ajey")``` or ```print('Ramanath')``` <br />

**Assigning the string value to variable**

* If we want to assign single line string to variable then we need to use single or double quotation marks after and before the string. <br />
		*Eg*: ```a = "Ajey Nayak"```

* If we want to assign multi line string to variable then we need to use three double quotation mark(""") or single quotation mark(''') <br />
		*Eg*: ```x = """My name is Ajey```<br />
						```I am learning python since 2 months``` <br />
						```I want to be come a successful Python - developer"""```<br />

**Python does not have character data type**

+ String are Arrays - If we want to access a element of the string the we can the index method inside the square bracket <br />
		*Eg*:  ```a = "Hello"``` <br />
			   ```print(a[1])``` *which display the character "e" as the string element start with index 0.

+ **Slicing** - If we want to access a set of element of the string. <br />
		*Eg*:  ```b = "Unglaublisch"``` <br />
				```print(b[2:7])``` *which the element "glaub" (from index 2 to 7*

+ **Negative Indexing** - if we want access last few elements of the string. <br />
		*Eg*:  ```c= "Meinung"``` <br />
				```print(c[-6:-1]``` *which displays "einung" (from index -5 to -1)*

+ **String Length** - If we want to find the length of the string, we can use **len()**  <br />
		*Eg*: ```d= "Ajeya Nayak"``` <br />
			  ```print(len(d))``` *which displays 11* 

**String Methods:**

+ **strip()** - which removes the space from begging or the end and which will not remove the space between two words. <br />
		*Eg*: ```a = "  Computer System"``` <br />
			  ```print(a.strip())``` *which shows as* **Computer System**
			  
+ **lower()** - which converts the string to lower case  <br />
		*Eg*:  ```a="Computer System"``` <br />
			   ```print(a.lower())``` *which shows as* **computer system**
			   
+ **upper()** - which converts the string to upper case  <br />
		*Eg*:  ```a="Computer System"``` <br />
			   ```print(a.upper())``` *which shows as* **COMPUTER SYSTEM**
			   
+ **replace** - which replace the character from one to another. and which is case sensitive <br />
		*Eg*:  ```b ="bellphone"``` <br />
			   ```print(b.replace("b","c")``` *which shows as* **cellphone** 
			   
+ **split** - which divides the string in two or more sub-string , if there is instances separator. <br />
		*Eg*:  ```c="Ajeya Nayak"``` <br />
			   ```print(c.split(" "))``` *which split into two sub-string with separator "," at last it shows ['Ajeya' , 'Nayak']*

+ check String - If we want to check the certain phrase or character present or not, We can use the keyword "in"  for present and "not in" for absent cases. <br />
	
	**For "in" cases** <br />
	```txt = " My town is karkala"``` <br />
	```x =  "karkala" in txt``` <br />
	```print(x)``` *which displays* **True** <br />
	```y= "city" in txt``` <br />
	```print(y)```  *which displays* **False**
     
	**For "not in" cases** <br />
	```cnt = "Electricity"``` <br />
	```a = "town" not in cnt``` <br />
	```print(a)``` *which shows* **True** <br />
	```b = "ect" not in cnt``` <br />
	```print(b)``` *which shows* **False**

**String Concatenation**

*we need to use + operator for merge two strings and this method will not support a string and an Integer* <br />
		*Eg*:	```a= "Uttar"``` <br />
				```b= " Pradesh"``` <br />
				```print(a + b)``` *which display value as* **Uttar Pradesh** 

**String Format**

* If we want to combine string and integer, Then we need to use* **format()** *method to concatenate.* <br />
		*Eg*:	```state = 31``` <br />
				```txt = "There are {} states in India"``` <br />
				```print(txt.format(state))``` *which display as* **There are 31 states in India**

* similarly,. if there are more than one Integer, <br />
		*Eg*:	```sta = 31``` <br />
				```cap = 3``` <br />
				```con=7``` <br />
				```txt="World has {} continent , There are {} states in India and Andhra Pradesh has {} capitals."``` <br />
				```print(txt.format(con,sta,cap))``` *which dispaly as* **World has 7 continent , There are 31 states in India and Andhra Pradesh has 3 capitals.**

***Escape Character**

+ If we want to insert special character  which are illegal in string i.e, "", **backspace** or **Newline**, Then we need to use \ before inserting special character <br />
		*Eg*: ```print("India\'s capital is New Delhi")``` *which displays output as* **India's capital is New Delhi**