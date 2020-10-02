# Dictionary -  a type of Data Collection


**Dictionary is collection which is unordered, changeable and indexed. which are written with curly bracket and have keys and values** <br />
	*Eg*:	```thisdict = {``` <br />
  			```"brand": "Ford",``` <br />
  			```"model": "Mustang",``` <br />
			```"year": 1964 <br />````
			```}``` <br />
			```print(thisdict)``` *which returns {"brand": "Ford", "model": "Mustang", "year": 1964}*

* Accessing Items in Dictionary - we can access the items in Dictionary by referring its key inside the square bracket <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```x = thisdict["brand"] # also we can use x = thisdict.get("brand")``` <br />
			```print(x)``` *which returns value as* **"Ford"**.

* check the number of items in Lists <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```print(len(thisdict))``` *which displays the value as* 3

* Change Values - we can change the values in Dictionary referring by the Key name <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```thisdict["year"] = 2018``` <br />
			```print(thisdict)``` *which returns* **{"brand": "Ford", "model": "Mustang", "year": 2018}**

* Adding Items - we can add the items in Dictionary by adding key and assigning values to it. <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```thisdict["color"] = "red"``` <br />
			```print(thisdict)``` <br />
			*which displays* **{'brand': 'Ford', 'model': 'Mustang', 'year': 1964, 'color': 'red'}**
			
**Removing items** <br />

+ **pop()** -  we can remove the items in dictionary using pop() method with specifying key name <br />	 
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```thisdict.pop("model")```<br />
			```print(thisdict)``` <br />
			*which displays* **{'brand': 'Ford', 'year': 1964}** 
 
+ **popitem()** -  If we want to remove last item in dictionary, we can use popitem() <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```thisdict.popitem()``` <br />
			```print(thisdict)``` <br />
			*which displays* **{'brand': 'Ford', 'model': 'Mustang'}**

+ **del()** - If we want to delete or remove specified key in dictionary, we can use del() <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```del thisdict["model"]``` *if we are not specifying key, it will delete whole dictionary* <br />
			```print(thisdict)``` <br />
			*which displays* **{'brand': 'Ford', 'year': 1964}** <br />

+ **clear()** - this method will clear all item in dictionary <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```thisdict.clear()``` <br />
			```print(thisdict)``` *which displays* **{}**

**Copy a Dictionary** <br />

+ **copy()** - we can copy the dictionary using copy() method  <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```mydict = thisdict.copy()``` <br />
			```print(mydict)``` 

+ **dict()** -  we can also copy the dictionary using dict method <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```mydict = dict(thisdict)``` <br />
			```print(mydict)```

**Loop Through a Dictionary** <br />

* If we want to display only keys , we can use the following method in dictionary <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```for x in thisdict:``` <br />
	  			```print(x)``` <br />
			*which displays keys in order* <br />
					**brand** <br />
					**model** <br />
					**year**

* If we want to display only values in dictionary <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```for x in thisdict:``` <br />
	  			```print(thisdict[x])``` <br />
			*which displays values in order* <br />
					**Ford** <br />
					**Mustang** <br />
					**1964**

* Also we can use value() method to get value in dictionary  <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```for x in thisdict.values:``` <br />
	  		```print(x)```  <br />
			*which displays values in order* <br />
				**Ford**  <br />
				**Mustang** <br />
				**1964**

* If we want to get both key and values, then we can use items() <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```for x, y in thisdict.items():``` <br />
  				```print(x, y)``` <br />
			*which displays Keys & values in order* <br />
				**brand Ford** <br />
				**model Mustang** <br />
				**year 1964** <br />

**Nested Dictionaries** <br />
		  
* If the dictionaries are under a dictionary we are calling it as Nested Dictionary <br />
	*Eg*:	```myfamily = {``` <br />
  			```"child1" : {``` <br />
		    ```"name" : "Emil",``` <br />
		    ```"year" : 2004``` <br />
			``` },``` <br />
		  	```"child2" : { ``` <br />
		    ```"name" : "Tobias",``` <br />
		    ```"year" : 2007``` <br />
		  ``` },``` <br />
		  ```"child3" : {``` <br />
	    ```"name" : "Linus",``` <br />
    	```"year" : 2011``` <br />
		  ```}``` <br />
		```}``` <br />
		```print(myfamily)``` <br />
		*which displays <br />
**{'child1': {'name': 'Emil', 'year': 2004}, 'child2': {'name': 'Tobias', 'year':2007}, 'child3': {'name': 'Linus', 'year': 2011}}**


* Check if Key exists  <br />
	*Eg*:	```thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}``` <br />
			```if "model" in thisdict:``` *where "model" is key in the dictionary* <br />
				```print("Yes, 'model' is one of the keys in the thisdict dictionary")```
