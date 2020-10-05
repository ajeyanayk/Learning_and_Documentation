<h1 align="Center">String Formating</h1>

* *format()* - If we want to resulted string to formatted as we expected

* If we the text is not defined or maybe come from database or user input  and we want to display those values in between any sentence. we can fill those space with {} (flower) brackets <br />
		*Eg*: 	
```python
				price = 49 
				txt = "The price is {} dollars" 
				print(txt.format(price))# formatting the value of {}
```

* If we want to format same value in float format <br />
	*Eg*:	
```python
			price = 49 
			txt = "The price is {:.2f} dollars" 
			// we have added .2f between {} to make the value as float 
			print(txt.format(price)) 
			//we will get  the result as The price is 49.00 dollars
```

| **Format** | **Description** |
|------------|--------------|
| :< | Left aligns the result (within the available space) |
| :> | Right aligns the result (within the available space) |
| :^ | Center aligns the result (within the available space) |
| := | Places the sign to the left most position |
| :+ | Use a plus sign to indicate if the result is positive or negative |
| :- | Use a minus sign for negative values only |
| : | Use a space to insert an extra space before positive numbers (and a minus sign before negative numbers) |
| :, | Use a comma as a thousand separator |
| :_ | Use a underscore as a thousand separator |
| :b | Binary format |
| :c | Converts the value into the corresponding Unicode character |
| :d | Decimal format |
| :e | Scientific format, with a lower case e |
| :E | Scientific format, with an upper case E |
|:f | Fix point number format |
|:F | Fix point number format, in uppercase format (show inf and nan as INF and NAN) |
|:g | General format |
|:G | General format (using a upper case E for scientific notations) |
|:o | Octal format|
|:x | Hex format, lower case |
|:X | Hex format, upper case |
| :n | Number format |
|:% | Percentage format |

* *Multiple Values* - If we want to display 2 or more value in sentence and the value will be filled as per the respective variable defined in format. <br />
	*Eg*:	
```python
				quantity = 3 
				itemno = 567 
				price = 49 
				myorder = "I want {} pieces of item number {} for {:.2f} dollars." 
				print(myorder.format(quantity, itemno, price)) 
				//first{} filled with quantity, second{} filled with itemno and last{} filled with price.
```

* If we want to display same value more than once or we want display not according to default format method. we can use index method <br />
	*Eg 1*:		
```python
				quantity = 3 
				itemno = 567 
				price = 49 
				myorder = "I want {0} pieces of item number {1} for {2:.2f} dollars." 
				print(myorder.format(quantity, itemno, price))
```

	Eg 2:		

```python			age = 36 
				name = "John" 
				txt = "His name is {1}. {1} is {0} years old." 
				`print(txt.format(age, name))`
```
				

**Named Indexes** <br />
* we can use named index instead of numeric index to avoid misunderstanding. <br />
	*Eg*:	
```python
			myorder = "I have a {carname}, it is a {model}." 
			print(myorder.format(carname = "Ford", model = "Mustang"))
```



