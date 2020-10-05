<h1 align="center">Classes and Object</h1>

A class is like an object constructor or a "blueprint" for creating objects

* *Create Class* - to create class , we need to use keyword "Class" <br />
	*Eg*:	
```python
			class Myclass:
				x = 5
```

* *Create Object* - We need to use class name to create Object <br />
	*Eg*:	
```python
			class Myclass: 
				x = 5 
		 
			p1 = MyClass() //p1 is object
			print(p1.x) //which displays value as 5
```

* *The __init__() function* - This function to assign values to object properties , or other operation that needs to do when object is created. <br />
	*Eg*:	
```python
			class Person: 
  				def __init__(self, name, age): 
   					self.name = name 
   					self.age = age 
		 
			p1 = Person("John", 36)  //p1 is object
			print(p1.name) 
			print(p1.age)
```

* *Object Methods* - Method are function which will take argument from Object. <br />
	*Eg*:	
```python
			class Person: 
			  	def __init__(self, name, age): 
			    		self.name = name 
			    		self.age = age 
			 
			  	def myfunc(self):  //method is working like function
			    		print("Hello my name is " + self.name) 
			 
			p1 = Person("John", 36)  //object 
			p1.myfunc() //calling method  //object with method which is calling method
```

* *The Self Parameter* - self parameter is reference to current instance of class and which is used access to variable that belongs to class.we can rename whatever we like. <br />
	*Eg*:	
```python
			class Person: 
			  	def __init__(mysillyobject, name, age):  //self parameter changed to mysillyobject
			    		mysillyobject.name = name 
			    		mysillyobject.age = age 
		 
			  	def myfunc(abc): *self parameter changed to abc* 
    					print("Hello my name is " + abc.name) 
		 
			p1 = Person("John", 36) 
			p1.myfunc()
```

* *Modify Object Properties* - If we want to modify any value in object. we can change  <br />
	Syntax:  `object.argname= modified value` <br />
	Eg:	
```python
			class Person: 
  				def __init__(self, name, age): 
					self.name = name 
					self.age = age 
		 
				def myfunc(self): 
			    print("Hello my name is " + self.name) 
		 
			p1 = Person("John", 36) //object construction 
			p1.age = 40 //object value modification 
			print(p1.age)
```

* *Delete object properties* - We can delete object properties using keyword del <br />
	*Eg*:	
```python
			class Person: 
				def __init__(self, name, age): 
					self.name = name 
					self.age = age 
		 
				def myfunc(self): 
					print("Hello my name is " + self.name) 
		 
			p1 = Person("John", 36) 
			del p1.age //deletion of object
			print(p1.age)
```

* *Del object* - we can delete object using keyword del <br />
	*Eg*:	
```python
			class Person: 
				def __init__(self, name, age): 
			    self.name = name 
			    self.age = age 
		 
				def myfunc(self): 
					print("Hello my name is " + self.name) 
   
			p1 = Person("John", 36) 
			del p1 
			print(p1)	
```

* *The pass statemet* - Once class is defined, and there is no content because of some reason and to avoid getting error message. we can type pass. <br />
  *Eg*:
```python
			class Person:
				pass
```
*having an empty class definition like this, would raise an error without the pass statement*