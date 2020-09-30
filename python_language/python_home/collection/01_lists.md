 Lists are collection which is ordered and changeable and written inside the square bracket.
	Eg:	 a=["Ajey", "Male","Karkala"]
				print(a) # which prints ["Ajey", "Male","Karkala"]

Access items- we can access the items in Lists referring indexing number.
	Eg:	 a=["Ajey", "Male","Karkala"]
				print(a[1]) # which prints "Male" as output.

to check the number of items in Lists
	Eg: 	thislist = ["apple", "banana", "cherry"]
			print(len(thislist) # which displays the value as 3

Negative Indexing - If we want to access last item or second last item , we access them using negative indexing. 
	Eg:	 a=["Ajey", "Male","Karkala"]
				print(a[-1]) # which prints "Karkala" as it is last position.
	
Range of indexing - 
If we want access particular sequence of items. we can access by from item to to item and insert colon icon between that.
	Eg:	 a=["Ajey", 29,"Male","Karkala","SBC"]
				print(a[1:3]) # which prints [29,"Male","Karkala"]

If we want the item from begging to till particular item, we can make empty at begging index and type end index number with colon
	Eg:	 a=["Ajey", 29,"Male","Karkala","SBC"]
				print(a[:3]) # which prints ["Ajey", 29,"Male","Karkala"]

If we want the item from particular item to till end, we need to type start index and end index should be blank with colon
	Eg:	 a=["Ajey", 29,"Male","Karkala","SBC"]
				print(a[1:]) # which prints [29,"Male","Karkala","SBC"]

Similarly, we can access items in sequence from last
	Eg:	 thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
			 print(thislist[-4:-1])# which prints ['orange', 'kiwi', 'melon']
			#the items from index -4 (included) to index -1 (excluded)

Change Item Value - If we want to change the item in list.
	Eg: 	thislist = ["apple", "banana", "cherry"]
			thislist[1] = "blackcurrant"
			print(thislist) # which prints ["apple", "blackcurrant", "cherry"]

append() - to add an item to the end of the list
	Eg:  	thislist = ["apple", "banana", "cherry"]
			thislist.append("orange")
			print(thislist) # which displays ['apple', 'banana', 'cherry', 'orange']

Insert() - to insert the item in specific index in the list
	Eg:  thislist = ["apple", "banana", "cherry"]
			thislist.insert(1, "orange") # 1 is index and "Orange" is item
			print(thislist) # which displays ['apple', 'orange', 'banana', 'cherry']

Remove() - to remove the items from lists
	Eg  thislist = ["apple", "banana", "cherry"]
		  thislist.remove("banana")
		  print(thislist) # which displays ['apple', 'cherry']

pop() - to remove the specified index or last item if index is not mentioned from lists
	Eg  thislist = ["apple", "banana", "cherry"]
		   thislist.pop()
			print(thislist) # which displays  ["apple", "banana"]

del() - to remove the specified index from lists or if index is not mentioned, the delete whole lists.
	Eg:  thislist = ["apple", "banana", "cherry"]
			del thislist[0]
			print(thislist) # which displays  ["banana", "cherry"]

clear() - which clear the whole list file 
	Eg:  thislist = ["apple", "banana", "cherry"]
			thislist.clear()
			print(thislist) # which displays  [] (empty lists)

copy() -  to copy the lists
	Eg: thislist = ["apple", "banana", "cherry"]
		  mylist = thislist.copy()
		  print(mylist) # which displays ["apple", "banana", "cherry"]

list() - another way to copy the lists
	Eg: 	thislist = ["apple", "banana", "cherry"]
			mylist = list(thislist)
			print(mylist)# which displays ["apple", "banana", "cherry"]

Join two lists - We can concatenate two list by 4 method

 Using + operator - we can concatenate two lists by + operator
	Eg: 	list1 = ["a", "b" , "c"]
			list2 = [1, 2, 3]
			list3 = list1 + list2
			print(list3)  # which returns ['a', 'b', 'c', 1, 2, 3]

append() 
	Eg:	list1 = ["a", "b" , "c"]
			list2 = [1, 2, 3]
			for x in list2:
 			list1.append(x)
			print(list1) # which returns ['a', 'b', 'c', 1, 2, 3]

extend()
	Eg:	list1 = ["a", "b" , "c"]
			list2 = [1, 2, 3]
			list1.extend(list2)
			print(list1) # which returns ['a', 'b', 'c', 1, 2, 3]

Loop through a List
 If we want to access item individually  ( without bracket) in order
Eg:		thislist = ["apple", "banana", "cherry"]
			for x in thislist:
  			print(x) 
			# which displays the value in order  
			"apple"
			"banana"
			"cherry"

 check if the item Exists 
Eg: 		thislist = ["apple", "banana", "cherry"]
			if "apple" in thislist:
  			print("Yes, 'apple' is in the fruits list")	


