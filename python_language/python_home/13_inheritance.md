# Inheritance

**Inheritance will take all the methods and properties from another class**

* Parent class - the class being inherited from, also called base class. <br />
* child class - the class that inherits from another class, also called derived class

**Create a Parent Class** <br />
* Parent class is the same as creating other class <br />
	*Eg*:	```class Person:``` <br />
			  ```def __init__(self, fname, lname):``` <br />
			    	```self.firstname = fname``` <br />
					```self.lastname = lname``` <br />
<br />		``` ```
			  ```def printname(self):``` <br />
				```print(self.firstname, self.lastname)``` <br />
<br />		``` ```
			```x = Person("John", "Doe")``` <br />
			```x.printname()```

**Create a Child Class** <br />
* If class is inherited from another class, which literally means opting functionality and method from base class <br />
	*Eg*:	```class Person:``` <br />
				```def __init__(self, fname, lname):``` <br />
					```self.firstname = fname``` <br />
					```self.lastname = lname``` <br />
<br />		``` ```
				```def printname(self):``` <br />
					```print(self.firstname, self.lastname)``` <br />
<br />		``` ```
			```class Student(Person):``` //child class with base class (inside bracket) <br />
				```pass``` <br />
<br />		``` ```
			```x = Student("Mike", "Olsen")``` <br />
			```x.printname()``` <br />

**Add the __init__() Function** <br />
* When we introduce __init__() functionality in child class, It overrides the existing base class. To over come from this issue add a call to parent <br />
	*Eg*:	```class Person:``` <br />
			  ```def __init__(self, fname, lname):``` <br />
			    ```self.firstname = fname``` <br />
			    ```self.lastname = lname``` <br />
<br />		``` ```
			  ```def printname(self):``` <br />
			    ```print(self.firstname, self.lastname)``` <br />
<br />		``` ```
			```class Student(Person):``` <br />
			  ```def __init__(self, fname, lname):``` //__init__() function of the child class <br />
			    ```Person.__init__(self, fname, lname)``` //calling base class __init__() function <br />
<br />		``` ```
			```x = Student("Mike", "Olsen")``` <br />
			```x.printname()```

**Use the Super() Function** <br />
* **Super()** function also inherit all method and functionality from base class. <br />
	*Eg*:	```class Person:``` <br />
			  ```def __init__(self, fname, lname):``` <br />
			    ```self.firstname = fname``` <br />
			    ```self.lastname = lname``` <br />
<br />		``` ```
			  ```def printname(self):``` <br />
			    ```print(self.firstname, self.lastname)``` <br />
<br />		``` ```
			```class Student(Person):``` <br />
			  ```def __init__(self, fname, lname):``` <br />
			    ```super().__init__(fname, lname)``` <br />
<br />		``` ```
			```x = Student("Mike", "Olsen")``` <br />
			```x.printname()```

**Add Properties** <br />
* If we want to add properties in child class , insert an line once after declaration with self. property with value  <br />
	*Eg*:	```class Person:``` <br />
			  ```def __init__(self, fname, lname):``` <br />
			    ```self.firstname = fname``` <br />
			    ```self.lastname = lname``` <br />
<br />		``` ```
			  ```def printname(self):``` <br />
			    ```print(self.firstname, self.lastname)``` <br />
<br />		``` ```
			```class Student(Person):``` <br />
			  ```def __init__(self, fname, lname):``` <br />
			    ```super().__init__(fname, lname)``` <br />
			    ```self.graduationyear = 2019``` //adding property <br />
<br />		``` ```
			```x = Student("Mike", "Olsen")``` <br />
			```print(x.graduationyear)```

**Add Method** //same like class, we can add in method <br />
	*Eg*:	```class Person:``` <br />
  				```def __init__(self, fname, lname):``` <br />
				    ```self.firstname = fname``` <br />
				    ```self.lastname = lname``` <br />
<br />		``` ```
			  	```def printname(self):``` <br />
				    ```print(self.firstname, self.lastname)``` <br />
<br />		``` ```
			```class Studnt(Person):``` <br />
			  ```def __init__(self, fname, lname, year):``` <br />
			    ```super().__init__(fname, lname)``` <br />
			    ```self.graduationyear = year``` <br />
<br />		``` ```
			  ```def welcome(self):``` <br />
			    ```print("Welcome", self.firstname, self.lastname, "to the class of",self.graduationyear)``` <br />
<br />		``` ```
			```x = Student("Mike", "Olsen", 2019)``` //object construction with child class``` <br />
			```x.welcome()``` //calling child class method

