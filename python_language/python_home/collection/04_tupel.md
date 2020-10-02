# Tuple -  a type of Data Collection

**Tuples are collection which are ordered and unchangeable and written with round bracket.** 
	*Eg*:	'''thistuple = ("apple", "banana", "cherry")'''
			'''print(thistuple) # which returns ("apple", "banana", "cherry")'''

**If we want to add or delete items from Tupels, we need to convert it to lists and we need to follow as in lists, using list()**

+ **Access Tuple items** - We can access the items in Tuple by indexing method <br />
 	*Eg*:	```thistuple = ("apple", "banana", "cherry")``` <br />
			```print(thistuple[1]) #which display "banana"``` <br />

+ **Negative Indexing** - If we want to access last item or second last item , we access them using negative indexing. <br />
	*Eg*:	 ```a=("Ajey", "Male","Karkala")``` <br />
			```print(a[-1]) # which prints "Karkala" as it is last position <br />```

+ **Range of indexing** - If we want access particular sequence of items. we can access by from item to to item and insert colon icon between that. <br />
	*Eg*:	```thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")``` <br />
			```print(thistuple[2:5])# which displays ("cherry", "orange", "kiwi")``` <br />
	*The search will start at index 2 (included) and end at index 5 (not included).* <br />

	* If we can access items in sequence from last <br />
		*Eg*:	```thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")``` <br />
				```print(thistuple[-4:-1])# which displays ('orange', 'kiwi', 'melon')``` <br />
	*This example returns the items from index -4 (included) to index -1 (excluded)* <br />

**Change Tuple value** <br />
*If we want to add or delete items from Tupels, we need to convert it to lists and we need to follow as in lists, using list()* <br />

**Loop through a List** <br />

+ If we want to access item individually ( without bracket) in order <br />
	*Eg*:	```thistuple = ("apple", "banana", "cherry")``` <br />
			```for x in thistuple:``` <br />
  				```print(x)``` <br />
			which displays the value in order <br />
				**"apple"** <br />
				**"banana"** <br />
				**"cherry"** <br />

+ check if the item Exists <br />
	*Eg*: 	```thistuple = ("apple", "banana", "cherry")``` <br />
			```if "apple" in thistuple:``` <br />
 					```print("Yes, 'apple' is in the fruits tuple")``` <br />

+ check the number of items in Tupels <br />
	*Eg*: 	```thistuple = ("apple", "banana", "cherry")``` <br />
			```print(len(thistuple))``` *which displays the value as* 3
