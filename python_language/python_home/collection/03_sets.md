Sets are collection, which are unordered and un-indexed and written with flower bracket
	Eg:		thisset = {"apple", "banana", "cherry"}
				print(thisset) # which returns {"apple", "banana", "cherry"}

Access items in Set
				we cannot access Set items like we will do in lists or tupels as which is not ordered or not indexed. But we can specify the value current status
	Eg:	thisset = {"apple", "banana", "cherry"}
			for x in thisset:
 			print(x) # which display {"apple", "banana", "cherry"}
In the above the example the item may change as items are not fixed.

check if the item Exists 	
	Eg:	thisset = {"apple", "banana", "cherry"}
			print("banana" in thisset)

to check the number of items in Set
	Eg: 	thisset = {"apple", "banana", "cherry"}
			print(len(thisset)) # which displays the value as 3

Add items 
		If we want to add to item to set,we can use add() and if we want to add more than 1 items then we can use update() method.
	Eg:	thisset = {"apple", "banana", "cherry"}
			thisset.add("orange")
			print(thisset)

			thisset = {"apple", "banana", "cherry"}
			thisset.update(["orange", "mango", "grapes"])
			print(thisset)

Remove items
		If we want to remove a item to set, we can use remove() or discard () method
	Eg:	thisset = {"apple", "banana", "cherry"}
			thisset.remove("banana") 
			# we can use discard()if remove() method doesn't exist, vice-versa
			print(thisset)
	
	we can also pop() to remove last item , But the set is not indexed, that's why it is not recommended.

clear() method is used to clear the items  in set
del() method is used to delete set completely

Set concatenation
union() or update() method to combine two sets
Eg:	set1 = {"a", "b" , "c"}
		set2 = {1, 2, 3}
		set3 = set1.union(set2)
		# we can use update() if union() method doesn't exist and vice-versa
		print(set3)
