# Scope

* **Local Scope** - If a variable defined inside function and it belongs to the local scope of that function. <br />
		*Eg*:	```def myfunc():``` <br />
	  				```x = 300``` //x is local scope <br />
					```print(x)``` <br />
<br />			``` ```
				```myfunc()```

* **Global Scope -  If a variable defined outside function and can be used by anyone.** <br />
	*Eg*:	```x = 300``` <br />
			```def myfunc():``` <br />
			  ```print(x)``` //which display value as 300 <br />
<br />			``` ```	
			```myfunc()``` <br />
			```print(x)``` //which display value as 300

* **Naming Variable** - If we assigned different value to variable with same name inside as well as out side function. Python will treat them as 2 variable. It will consider Global scope variable for outside function and inside the function as local scope. <br />
	*Eg*:	```x=300```	//Global scope <br />
			```def myfunc():``` <br />
		  		```x = 200``` //Local scope <br />
		  		```print(x)``` //which display value as 200 <br />
<br />			``` ```
			```myfunc()``` <br />
			```print(x)``` //which display value as 300

* **Global keyword** - If a variable defined inside function and we want to make global use , Then we need add global Keyword before variable. <br />
	*Eg*:	```def myfunc():``` <br />
			  	```global x```  //marking variable with global scope <br />
		  		```x = 300``` <br />
<br />			``` ```
			```myfunc()``` <br />
			```print(x)```