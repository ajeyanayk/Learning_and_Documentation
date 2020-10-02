Dictionary is collection which is unordered, changeable and indexed. which are written with curly bracket and have keys and values
	Eg:		thisdict = {
  				"brand": "Ford",
  				"model": "Mustang",
				  "year": 1964
				 }
				print(thisdict) # which returns {"brand": "Ford", "model": "Mustang", "year": 1964}

Accessing Items in Dictionary
 		we can access the items in Dictionary by referring its key inside the square bracket
	Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
				x = thisdict["brand"] # also we can use x = thisdict.get("brand")
				print(x) # which returns value as "Ford".

to check the number of items in Lists
Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
			print(len(thisdict)) # which displays the value as 3

Change Values
		we can change the values in Dictionary referring by the Key name
	Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
				thisdict["year"] = 2018
				print(thisdict)# which returns {"brand": "Ford", "model": "Mustang", "year": 2018}

 Adding Items
		we can add the items in Dictionary by adding key and assigning values to it.
Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
			thisdict["color"] = "red"
			print(thisdict) 
			# which displays {'brand': 'Ford', 'model': 'Mustang', 'year': 1964, 'color': 'red'}

Removing items
pop() -  we can remove the items in dictionary using pop() method with specifying 		   key name 	
Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
			thisdict.pop("model")
			print(thisdict)
			# which displays {'brand': 'Ford', 'year': 1964}

popitem()-  If we want to remove last item in dictionary, we can use popitem()
Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
			thisdict.popitem()
			print(thisdict)
			# which displays {'brand': 'Ford', 'model': 'Mustang'}

del() - If we want to delete or remove specified key in dictionary, we can use del()
Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
			del thisdict["model"] # if we are not specifying key, it will delete whole dictionary
			print(thisdict)
			# which displays {'brand': 'Ford', 'year': 1964}

clear() - this method will clear all item in dictionary
Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
			thisdict.clear()
			print(thisdict) # which displays {}

Copy a Dictionary
copy()- we can copy the dictionary using copy() method 
Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
			mydict = thisdict.copy()
			print(mydict)

dict() -  we can also copy the dictionary using dict method
Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
			mydict = dict(thisdict)
			print(mydict)

Loop Through a Dictionary
If we want to display only keys , we can use the following method in dictionary
	Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
				for x in thisdict:
	  			print(x)
				# which displays keys in order
					brand
					model
					year

If we want to display only values in dictionary
	Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
				for x in thisdict:
	  			print(thisdict[x])
				# which displays values in order
					Ford
					Mustang
					1964

Also we can value() method to get value in dictionary
Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
			for x in thisdict.values:
	  		print(x)
			# which displays values in order
				Ford
				Mustang
				1964

If we want to get both key and values, then we can use items()
Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
			for x, y in thisdict.items():
  			print(x, y)
			# which displays Keys & values in order
			brand Ford
			model Mustang
			year 1964

 Nested Dictionaries
		  If the dictionaries are under a dictionary we are calling it as Nested Dictionary
Eg:		myfamily = {
  			"child1" : {
		    "name" : "Emil",
		    "year" : 2004
			 },
		  	"child2" : {
		    "name" : "Tobias",
		    "year" : 2007
		   },
		  "child3" : {
	    "name" : "Linus",
    	"year" : 2011
		  }
		}
		print(myfamily)
		#which displays
{'child1': {'name': 'Emil', 'year': 2004}, 'child2': {'name': 'Tobias', 'year':2007}, 'child3': {'name': 'Linus', 'year': 2011}}


 Check if Key exists 
Eg:		thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}
			if "model" in thisdict: # where "model" is key in th
			print("Yes, 'model' is one of the keys in the thisdict dictionary")
