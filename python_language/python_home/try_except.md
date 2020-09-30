When an error occurs or exception and we want to stop and generate an error messages
We have three keywords to block and generate an error message
try - which blocks and generate an exception
except -  which blocks and handle error
finally	-  it allows  execute the code irrespective of try or except blocks.

Exception Handling
Eg: 		try:
 		 		print(x) # try will generate an exception as x is not defined
			except:
 		 		print("An exception occurred") 
		# exception blocks and show error message if mentioned.

Many Exception
		we can generate many exception blocks as we want.
Eg:		try:
			  print(x)
			except NameError: 
			  print("Variable x is not defined")
			except:
			  print("Something else went wrong")

Else -   we can use the else keyword , if there is no error were raised.
Eg:		try:
 			 print("Hello")
			except:
			  print("Something went wrong")
			else:
			  print("Nothing went wrong")

finally - If finally block specified, will be executed whether try or except will raise an error or not
Eg 1 :		try:
			  print(x) # try will generate an exception as x is not defined
			except:
			  print("Something went wrong") 
			#As exception created will generate an error message 
			finally:
			  print("The 'try except' is finished")

Eg 2 : 		try:
				  f = open("demofile.txt")
				  f.write("Lorum Ipsum")
				except:
				  print("Something went wrong when writing to the file")
				finally:
				  f.close()

Raise an exception
		if any error occurs during any condition, we can raise an exception by throwing an error.
Eg 1 :	x = -1
			if x < 0:
			  raise Exception("Sorry, no numbers below zero")	



