# Collection _ introduction

### There are four type of collecting data structure in Python

1. **List** is a collection which is ordered and changeable. Allows duplicate members.
2. **Tuple** is a collection which is ordered and unchangeable. Allows duplicate members.
3. **Set** is a collection which is unordered and un-indexed. No duplicate members.
4. **Dictionary** is a collection which is unordered, changeable and indexed. No duplicate members.

#### **List** <br />
* If we want to convert from tuples to lists ,we need to use list() <br />
 *Eg*: 	```a = ("apple", "banana", "cherry")``` <br />
		   ```thislist = list(a)``` <br />
		   ```print(thislist)``` <br />
	      *which displays item with square bracket(Lists)* **["apple", "banana", "cherry"]**

#### **Tuple** <br />
* If we want to convert from lists to tuples ,we need to use tupel() <br />
 *Eg*: 	```b = ["apple", "banana", "cherry"]``` <br />			
		    ```thistupel = tupel(b)``` <br />
		   ```print(thistupel)``` <br />
		   *which displays item with  bracket (tupels)* **("apple", "banana", "cherry")** <br />

#### **Set** <br />
+ If we want construct or convert from lists or tuples to set, we need to use set() <br />
*Eg*:	```c = ("apple", "banana", "cherry")``` <br />
		```thisset = set(c)``` <br />
		```print(thisset)``` <br />
		   *which displays item with  curly bracket (set)* **{"apple", "banana", "cherry"}** <br />

#### **Dictionary** <br />
+ If we want to create dictionary from input, we can use dict() <br />
*Eg*:	```d= dict(brand="Ford", model="Mustang", year=1964)``` <br />
      ```print(d) ``` <br />
		 *note that keywords are not string literals and the use of equals rather than colon for the assignment and which displays Keys and values with curly bracket* 
		   **{"brand": "Ford", "model": "Mustang", "year": 1964}**
