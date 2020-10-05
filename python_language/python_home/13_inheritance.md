<h1 align="center">Inheritance</h1>

Inheritance will take all the methods and properties from another class

* Parent class - the class being inherited from, also called base class. <br />
* child class - the class that inherits from another class, also called derived class

* *Create a Parent Class* - Parent class is the same as creating other class <br />
	*Eg*:	
```python
		class Person: 
			def __init__(self, fname, lname): 
				self.firstname = fname 
				self.lastname = lname 
		 
			def printname(self): 
				print(self.firstname, self.lastname) 
		 
		x = Person("John", "Doe") 
		x.printname()
```

* *Create a Child Class* - If class is inherited from another class, which literally means opting functionality and method from base class <br />
	*Eg*:	
```python
		class Person: 
			def __init__(self, fname, lname): 
				self.firstname = fname 
				self.lastname = lname 
		 
			def printname(self): 
				print(self.firstname, self.lastname) 
		 
		class Student(Person): //child class with base class (inside bracket) 
			pass 
		 
		x = Student("Mike", "Olsen") 
		x.printname() 
```
* *Add the __init__() Function* - When we introduce __init__() functionality in child class, It overrides the existing base class. To over come from this issue add a call to parent <br />
	*Eg*:	

```python
		class Person: 
			def __init__(self, fname, lname): 
				self.firstname = fname 
			    self.lastname = lname 
		 
			def printname(self): 
			    print(self.firstname, self.lastname) 
		 
		class Student(Person): 
			def __init__(self, fname, lname): //__init__() function of the child class 
				Person.__init__(self, fname, lname) //calling base class __init__() function 
		 
		x = Student("Mike", "Olsen") 
		x.printname()
```
* *Use the Super() Function* - This function also inherit all method and functionality from base class. <br />
	*Eg*:	
```python
		class Person: 
			def __init__(self, fname, lname): 
				self.firstname = fname 
			    self.lastname = lname 
		 
			def printname(self): 
			    print(self.firstname, self.lastname) 
		 
		class Student(Person): 
			def __init__(self, fname, lname): 
				super().__init__(fname, lname) 
		 
		x = Student("Mike", "Olsen") 
		x.printname()
```

* *Add Properties* - If we want to add properties in child class , insert an line once after declaration with self. property with value  <br />
	*Eg*:	
```python
		class Person: 
			def __init__(self, fname, lname): 
				self.firstname = fname 
			    self.lastname = lname 
		 
			def printname(self): 
			    print(self.firstname, self.lastname) 
		 
		class Student(Person): 
			def __init__(self, fname, lname): 
			    super().__init__(fname, lname) 
			    self.graduationyear = 2019 //adding property 
		 
		x = Student("Mike", "Olsen") 
		print(x.graduationyear)
```
**Add Method** //same like class, we can add in method <br />
	*Eg*:	
```python
		class Person: 
  			def __init__(self, fname, lname): 
				self.firstname = fname 
				self.lastname = lname 
		 
			def printname(self): 
				print(self.firstname, self.lastname) 
		 
		class Studnt(Person): 
			def __init__(self, fname, lname, year): 
				super().__init__(fname, lname) 
			    self.graduationyear = year 
		 
			def welcome(self): 
			    print("Welcome", self.firstname, self.lastname, "to the class of",self.graduationyear) 
		 
		x = Student("Mike", "Olsen", 2019) //object construction with child class 
		x.welcome() //calling child class method

```