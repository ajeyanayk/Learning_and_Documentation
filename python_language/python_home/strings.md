String are surrounded by double quotation or single quotation mark
Eg: "Ajey"  or 'Ramanath'
we can display as 
print("Ajey") or print('Ramanath')

 Assigning the string value to variable
If we want to assign single line string to variable then we need to use single or double quotation marks after and before the string.
		Eg : a = "Ajey Nayak"

If we want to assign multi line string to variable then we need to use three double quotation mark(""") or single quotation mark(''')
		Eg: x = """My name is Ajey
							I am learning python since 2 months 
							I want to be come a successful Python - developer"""

Python does not have character data type,

String are Arrays-If we want to access a element of the string the we can the index method inside the square bracket
		Eg:  a = "Hello"
				print(a[1]) # which display the character "e"
									as the string element start with index 0.

Slicing - 	If we want to access a set of element of the string.
		Eg:  b = "Unglaublisch"
				print(b[2:7]) # which the element "glaub" (from index 2 to 7)

Negative Indexing - if we want access last few elements of the string.
		Eg:  c= "Meinung"
				print(c[-6:-1] # which displays "einung" (from index -5 to -1)

String Length - If we want to find the length of the string, we can use len() 
		Eg: d= "Ajeya Nayak"
				print(len(d)) # which displays 11 

String Methods:

strip() - which removes the space from begging or the end and which will not remove the space between two words.
		Eg : a = "  Computer System"
				print(a.strip()) # which shows as "Computer System"
lower()- which converts the string to lower case 
		Eg:  a="Computer System"
				 print(a.lower()) # which shows as "computer system"
upper() -which converts the string to upper case 
		Eg:  a="Computer System"
				print(a.upper()) # which shows as "COMPUTER SYSTEM"
replace - which replace the character from one to another. and which is case sensitive
		Eg:  b ="bellphone" 
				 print(b.replace("b","c") # which shows as "cellphone"
split - which divides the string in two or more sub-string , if there is instances separator.
		Eg:  c="Ajeya Nayak"
				 print(c.split(" ")) # which split into two sub-string with separator ","
											 at last it shows ['Ajeya' , 'Nayak']

check String 
		If we want to check the certain phrase or character present or not
    We can use the keyword "in"  for present and "not in" for absent cases.
Eg: 	
			For "in" cases
					txt = " My town is karkala"
					x =  "karkala" in txt
					print(x) #  which displays "True"
					y= "city" in txt
					print(y)  # which displays "False"
     
			For "not in" cases
					cnt = "Electricity"
					a = "town" not in cnt
					print(a) # which shows "True"
					b = "ect" not in cnt
					print(b) # which shows "False"

String Concatenation 
	we need to use + operator for merge two strings and this method will not support a string and an Integer
		Eg:		a= "Uttar"
					b= " Pradesh"
					print(a + b) # which display value as "Uttar Pradesh"

String Format
	If we want to combine string and integer, Then we need to use format() method to concatenate.
		Eg:		state = 31
					txt = "There are {} states in India"
					print(txt.format(state)) 
# which display as There are 31 states in India

similarly,. if there are more than one Integer,
					sta = 31
					cap = 3
					con=7
					txt="World has {} continent , There are {} states in India and Andhra Pradesh has {} capitals."
					print(txt.format(con,sta,cap)) 
# which dispaly as World has 7 continent , There are 31 states in India and Andhra Pradesh has 3 capitals.

Escape Character
	If we want to insert special character  which are illegal in string   					Eg: "",backspace or Newline, Then we need to use \ before inserting special character
		Eg: print("India\'s capital is New Delhi") 
# which displays output as India's capital is New Delhi