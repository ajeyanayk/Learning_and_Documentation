# List -  a type of Data Collection

**Lists are collection which is ordered and changeable and written inside the square bracket.** <br />
	*Eg*:	 ```a=["Ajey", "Male","Karkala"]``` <br />
				```print(a)```  *which prints* **["Ajey", "Male","Karkala"]**

* Access items- we can access the items in Lists referring indexing number. <br />
	*Eg*:	 ```a=["Ajey", "Male","Karkala"]``` <br />
				```print(a[1])``` *which prints **Male**  as output*.

* Check the number of items in Lists * <br />
	*Eg*: 	```thislist = ["apple", "banana", "cherry"]``` <br />
			```print(len(thislist)``` *which displays the value as* 3

* **Negative Indexing** - If we want to access last item or second last item , we access them using negative indexing. <br />
	*Eg*:	 ```a=["Ajey", "Male","Karkala"]``` <br />
				```print(a[-1])``` *which prints **Karkala** as it is last position*. <br />
	
* **Range of indexing** -  <br />
	+ If we want access particular sequence of items. we can access by from item to to item and insert colon icon between that. <br />
		*Eg*:	 ```a=["Ajey", 29,"Male","Karkala","SBC"]``` <br />
					```print(a[1:3])``` *which prints* **[29,"Male","Karkala"]** <br />

	+ If we want the item from begging to till particular item, we can make empty at begging index and type end index number with colon <br />
		*Eg*:	 ```a=["Ajey", 29,"Male","Karkala","SBC"]``` <br />
				```print(a[:3])```  *which prints* **["Ajey", 29,"Male","Karkala"]** <br />

	+ If we want the item from particular item to till end, we need to type start index and end index should be blank with colon <br />
		*Eg*:	 ```a=["Ajey", 29,"Male","Karkala","SBC"]``` <br />
				```print(a[1:])``` *which prints* **[29,"Male","Karkala","SBC"]** <br />

	+ If we can access items in sequence from last <br />
		*Eg*:	 ```thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]``` <br />
				```print(thislist[-4:-1])``` <br />
				*which prints* **['orange', 'kiwi', 'melon']**  and *the items from index -4 (included) to index -1 (excluded)* <br />

	+ Change Item Value - If we want to change the item in list. <br />
		*Eg*: 	```thislist = ["apple", "banana", "cherry"]``` <br />
				```thislist[1] = "blackcurrant"```<br />
				```print(thislist)``` *which prints* **["apple", "blackcurrant", "cherry"]** <br />

+ **append()** - to add an item to the end of the list <br />
	*Eg*:  	```thislist = ["apple", "banana", "cherry"]``` <br />
			```thislist.append("orange")``` <br />
			```print(thislist)``` *which displays* **['apple', 'banana', 'cherry', 'orange']** <br />

+ **insert()** - to insert the item in specific index in the list <br />
	*Eg*:  ```thislist = ["apple", "banana", "cherry"]``` <br />
			```thislist.insert(1, "orange")``` # 1 is index and "Orange" is item <br />
			```print(thislist)``` *which displays* **['apple', 'orange', 'banana', 'cherry']** <br />

+ **remove()** - to remove the items from lists <br />
	*Eg*:  ```thislist = ["apple", "banana", "cherry"]``` <br />
		  ```thislist.remove("banana")``` <br />
		  ```print(thislist)``` *which displays* **['apple', 'cherry']** <br />

+ **pop()** - to remove the specified index or last item if index is not mentioned from lists <br />
	*Eg*:  ```thislist = ["apple", "banana", "cherry"]``` <br />
		   ```thislist.pop()``` <br />
			```print(thislist)``` *which displays* **["apple", "banana"]** <br />

+ **del()** - to remove the specified index from lists or if index is not mentioned, the delete whole lists. <br />
	*Eg*:  ```thislist = ["apple", "banana", "cherry"]``` <br />
			```del thislist[0]``` <br />
			```print(thislist)``` *which displays* **["banana", "cherry"]** <br />

+ **clear()** - which clear the whole list file <br />
	*Eg*:  ```thislist = ["apple", "banana", "cherry"]``` <br />
			```thislist.clear()``` <br />
			```print(thislist)``` *which displays*  **[]** *(empty lists)* <br />

+ **copy()** -  to copy the lists <br />
	*Eg*: ```thislist = ["apple", "banana", "cherry"]``` <br />
		  ```mylist = thislist.copy()``` <br />
		  ```print(mylist)``` *which displays* **["apple", "banana", "cherry"]** <br />

+ **list()** - another way to copy the lists <br />
	*Eg*: 	```thislist = ["apple", "banana", "cherry"]``` <br />
			```mylist = list(thislist)``` <br />
			```print(mylist)``` *which displays* **["apple", "banana", "cherry"]** <br />

**Join two lists - We can concatenate two list by 4 method** <br />

	* Using *+* operator - we can concatenate two lists by + operator <br />
		*Eg*: 	```list1 = ["a", "b" , "c"]``` <br />
				```list2 = [1, 2, 3]``` <br />
				```list3 = list1 + list2``` <br />
				```print(list3)```  *which returns* **['a', 'b', 'c', 1, 2, 3]** <br />

	+ **append()** <br />
		*Eg*:	```list1 = ["a", "b" , "c"]``` <br />
				```list2 = [1, 2, 3]``` <br />
				```for x in list2:``` <br />
 					```list1.append(x)``` <br />
					```print(list1)``` *which returns* **['a', 'b', 'c', 1, 2, 3]** <br />

	+ **extend()** <br />
		*Eg*:	```list1 = ["a", "b" , "c"]``` <br />
				```list2 = [1, 2, 3]``` <br />
				```list1.extend(list2)``` <br />
				```print(list1)``` *which returns* **['a', 'b', 'c', 1, 2, 3]** <br />

**Loop through a List**

+ If we want to access item individually  ( without bracket) in order <br />
	*Eg*: ```thislist = ["apple", "banana", "cherry"]``` <br />
		   ```for x in thislist:``` <br />
				```print(x)``` <br />
			*which displays the value in order* <br /> 
				**"apple"** <br />
				**"banana"** <br />
				**"cherry"** <br />

+ check if the item Exists <br />
	*Eg*: ```thislist = ["apple", "banana", "cherry"]```<br />
		  ```if "apple" in thislist:``` <br />
  		  ```print("Yes, 'apple' is in the fruits list")``` <br />


