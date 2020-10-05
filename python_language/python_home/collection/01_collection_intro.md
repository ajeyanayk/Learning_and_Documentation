<h1 align="center">Collection _ introduction</h1>

**There are four type of collecting data structure in Python**

1. *List* is a collection which is ordered and changeable. Allows duplicate members.
2. *Tuple* is a collection which is ordered and unchangeable. Allows duplicate members.
3. *Set* is a collection which is unordered and un-indexed. No duplicate members.
4. *Dictionary* is a collection which is unordered, changeable and indexed. No duplicate members.

* *List* - If we want to convert from tuples to lists ,we need to use list() <br />
 *Eg*: 	
```python
a = ("apple", "banana", "cherry") 
thislist = list(a) 
print(thislist) 
//which displays item with square bracket(Lists)["apple", "banana", "cherry"]
```

* *Tuple* - If we want to convert from lists to tuples ,we need to use tupel() <br />
 *Eg*: 	
```python
b = ["apple", "banana", "cherry"] 			
thistupel = tupel(b) 
print(thistupel) 
//which displays item with  bracket (tupels) ("apple", "banana", "cherry")
```

* *Set* - If we want construct or convert from lists or tuples to set, we need to use set() <br />
*Eg*:	
```python
c = ("apple", "banana", "cherry") 
thisset = set(c) 
print(thisset) 
//which displays item with  curly bracket (set) {"apple", "banana", "cherry"}
```

* *Dictionary* - If we want to create dictionary from input, we can use dict() <br />
*Eg*:	
```python
d= dict(brand="Ford", model="Mustang", year=1964) 
print(d)  
// note that keywords are not string literals and the use of equals rather than colon for the assignment
// which displays Keys and values with curly bracket
{"brand": "Ford", "model": "Mustang", "year": 1964}
```