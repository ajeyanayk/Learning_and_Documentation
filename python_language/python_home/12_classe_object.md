# Classes and Object

**A class is like an object constructor or a "blueprint" for creating objects**

**Create Class** <br />
* To create class , we need to use keyword "Class" <br />
	*Eg*:	```class Myclass: <br />
				```x = 5

**Create Object** <br />
* We need to use class name to create Object <br />
	*Eg*:	```class Myclass:``` <br />
				```x = 5``` <br />
<br />		``` ```
			```p1 = MyClass()``` *p1 is object* <br />
			```print(p1.x)``` *which displays value as 5* 

**The __init__() function** <br />
* The __init__() function to assign values to object properties , or other operation that needs to do when object is created. <br />
	*Eg*:	```class Person:``` <br />
  				```def __init__(self, name, age):``` <br />
   					```self.name = name``` <br />
   					```self.age = age``` <br />
<br />		``` ```
			```p1 = Person("John", 36)```  *p1 is object* <br />
			```print(p1.name)``` <br />
			```print(p1.age)```

**Object Methods** <br />
* Method are function which will take argument from Object. <br />
	*Eg*:	```class Person:``` <br />
			  	```def __init__(self, name, age):``` <br />
			    	```self.name = name``` <br />
			    	```self.age = age``` <br />
<br />			``` ```
			  	```def myfunc(self):``` *method is working like function* <br />
			    	```print("Hello my name is " + self.name)``` <br />
<br />			``` ```
			```p1 = Person("John", 36)``` //object <br />
			```p1.myfunc()``` //calling method *object with method which is calling method* 

**The Self Parameter** <br />
* self parameter is reference to current instance of class and which is used access to variable that belongs to class.we can rename whatever we like. <br />
	*Eg*:	```class Person:``` <br />
			  	```def __init__(mysillyobject, name, age):``` *self parameter changed to mysillyobject* <br />
			    	```mysillyobject.name = name``` <br />
			    	```mysillyobject.age = age``` <br />
<br />		``` ```
			  	```def myfunc(abc):``` *self parameter changed to abc* <br />
    				```print("Hello my name is " + abc.name)``` <br />
<br />		``` ```
			```p1 = Person("John", 36)``` <br />
			```p1.myfunc()```

**Modify Object Properties** <br />
* If we want to modify any value in object. we can change  <br />
	Syntax:  ```object.argname= modified value```

	*Eg*:	```class Person:``` <br />
  				```def __init__(self, name, age):``` <br />
					```self.name = name``` <br />
					```self.age = age``` <br />
<br />		``` ```
				```def myfunc(self):``` <br />
			    ```print("Hello my name is " + self.name)``` <br />
<br />		``` ```
			```p1 = Person("John", 36)``` *object construction* <br />
			```p1.age = 40``` *object value modification* <br />
			```print(p1.age)```

**Delete object properties** <br />
* We can delete object properties using keyword del <br />
	*Eg*:	```class Person:``` <br />
				```def __init__(self, name, age):``` <br />
					```self.name = name``` <br />
					```self.age = age``` <br />
<br />		``` ```
				```def myfunc(self):``` <br />
					```print("Hello my name is " + self.name)``` <br />
<br />		``` ```
			```p1 = Person("John", 36)``` <br />
			```del p1.age``` *deletion of object* <br />
			```print(p1.age)```

**Del object** <br />
* we can delete object using keyword del <br />
	*Eg*:	```class Person:``` <br />
				```def __init__(self, name, age):``` <br />
			    ```self.name = name``` <br />
			    ```self.age = age``` <br />
<br />		``` ```
				```def myfunc(self):``` <br />
					```print("Hello my name is " + self.name)``` <br />
<br />  ``` ```
			```p1 = Person("John", 36)``` <br />
			```del p1``` <br />
			```print(p1)```	

**The pass statemet** <br />
* Once class is defined, and there is no content because of some reason and to avoid getting error message. we can type pass. <br />
	*Eg*:	```class Person:``` <br />
					```pass``` <br />
**having an empty class definition like this, would raise an error without the pass statement**