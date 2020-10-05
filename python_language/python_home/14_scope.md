<h1 align="center">Scope</h1>

* *Local Scope* - If a variable defined inside function and it belongs to the local scope of that function. <br />
		*Eg*:	
```python
			def myfunc(): 
	  			x = 300 //x is local scope 
				print(x) 
			 
			myfunc()
```

* *Global Scope* -  If a variable defined outside function and can be used by anyone. <br />
	*Eg*:	
```python
			x = 300 
			def myfunc(): 
			  print(x) //which display value as 300 
			 	
			myfunc() 
			print(x) //which display value as 300
```

* *Naming Variable* - If we assigned different value to variable with same name inside as well as out side function. Python will treat them as 2 variable. It will consider Global scope variable for outside function and inside the function as local scope. <br />
	*Eg*:	
```python
			x=300	//Global scope 
			def myfunc(): 
		  		x = 200 //Local scope 
		  		print(x) //which display value as 200 
			 
			myfunc() 
			print(x) //which display value as 300
```

* *Global keyword* - If a variable defined inside function and we want to make global use , Then we need add global Keyword before variable. <br />
	*Eg*:	
```python
			def myfunc(): 
			  	global x  //marking variable with global scope 
		  		x = 300 
			 
			myfunc() 
			print(x)
```