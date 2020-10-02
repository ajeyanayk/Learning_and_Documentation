Tuples are collection which are ordered and unchangeable and written with round bracket.
Eg:		thistuple = ("apple", "banana", "cherry")
			print(thistuple) # which returns ("apple", "banana", "cherry")

If we want to add or delete items from Tupels, we need to convert it to lists and we need to follow as in lists, using list()

Access Tuple items - We can access the items in Tuple by indexing method
 		Eg:		thistuple = ("apple", "banana", "cherry")
			print(thistuple[1]) #which display "banana"

Negative Indexing - If we want to access last item or second last item , we access them using negative indexing.
		Eg:	 	a=("Ajey", "Male","Karkala")
				print(a[-1]) # which prints "Karkala" as it is last position

Range of indexing -
		If we want access particular sequence of items. we can access by from item to to item 	and insert colon icon between that.
		Eg:		thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
					print(thistuple[2:5])# which displays ("cherry", "orange", "kiwi")
		# The search will start at index 2 (included) and end at index 5 (not included).

		If we can access items in sequence from last
		Eg:		thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
					print(thistuple[-4:-1])# which displays ('orange', 'kiwi', 'melon')
		#This example returns the items from index -4 (included) to index -1 (excluded)

Change Tuple value
If we want to add or delete items from Tupels, we need to convert it to lists and we need to follow as in lists, using list()

Loop through a List
 If we want to access item individually ( without bracket) in order
Eg:		thistuple = ("apple", "banana", "cherry")
			for x in thistuple:
  			print(x)
			# which displays the value in order
			"apple"
			"banana"
			"cherry"

 check if the item Exists 
Eg: 		thistuple = ("apple", "banana", "cherry")
			if "apple" in thistuple:
 			print("Yes, 'apple' is in the fruits tuple")

to check the number of items in Tupels
	Eg: 	thistuple = ("apple", "banana", "cherry")
			print(len(thistuple)) # which displays the value as 3
