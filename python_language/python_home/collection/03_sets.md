# Set -  a type of collection of data

**Sets are collection, which are unordered and un-indexed and written with flower bracket** <br />
	*Eg*:	```thisset = {"apple", "banana", "cherry"}``` <br />
			```print(thisset) # which returns {"apple", "banana", "cherry"}``` <br />

+ Access items in Set - we cannot access Set items like we will do in lists or tupels as which is not ordered or not indexed. But we can specify the value current status <br />
	*Eg*:	```thisset = {"apple", "banana", "cherry"}``` <br />
			```for x in thisset:``` <br />
 			```print(x)``` *which display* **{"apple", "banana", "cherry"}** <br />
*In the above the example the item may change as items are not fixed.** <br />

+ check if the item Exists 	<br />
	*Eg*:	```thisset = {"apple", "banana", "cherry"}``` <br />
			```print("banana" in thisset)``` <br />

+ check the number of items in Set <br />
	*Eg*: 	```thisset = {"apple", "banana", "cherry"}``` <br />
			```print(len(thisset))``` *which displays the value as* 3 <br />

+ **add()**  - If we want to add to item to set,we can use add() and if we want to add more than 1 items then we can use update() method. <br />
	*Eg*:	```thisset = {"apple", "banana", "cherry"}``` <br />
			```thisset.add("orange")``` <br />
			```print(thisset)``` <br />
      ```thisset = {"apple", "banana", "cherry"}``` <br />
			```thisset.update(["orange", "mango", "grapes"])``` <br />
			```print(thisset)``` <br />

+ **remove()** - If we want to remove a item to set, we can use **remove()** or **discard()** method <br />
	*Eg*:	```thisset = {"apple", "banana", "cherry"}``` <br />
			```thisset.remove("banana")``` <br />
			*we can use discard()if remove() method doesn't exist, vice-versa* <br />
			```print(thisset)``` <br />
			
*we can also **pop()** to remove last item , But the set is not indexed, that's why it is not recommended.* <br />

+ **clear()** - is used to clear the items  in set <br />
+ **del()** - is used to delete set completely <br />

**Set concatenation**

**union()** or **update()** method to combine two sets <br />
*Eg*:	```set1 = {"a", "b" , "c"}``` <br />
		```set2 = {1, 2, 3}``` <br />
		```set3 = set1.union(set2)``` <br />
		*we can use update() if union() method doesn't exist and vice-versa* <br />
		```print(set3)``` <br />
