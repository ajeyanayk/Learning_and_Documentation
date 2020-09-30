for loop is used for iterating over sequence (that is either a list, a tuple, a dictionary, a set, or a string).
Eg:		fruits = ["apple", "banana", "cherry"]
			for x in fruits:
  			print(x)
# which displays fruits name in order like
		apple
		banana
		cherry

If the object is string, then it display individual character
Eg:	for x in "banana":
 			print(x)	
# which displays fruits name in order like
				b
				a
				n
				a
				n
				a

Break Statement - like in while loop, we can stop the loop even though statement is true using break statement
Eg:		fruits = ["apple", "banana", "cherry"]
			for x in fruits:
			  print(x)
				if x == "banana":
			    	break 
# which displays fruits name in order like
				apple
				banana

continue statement - like in while loo, we can stop current iteration and continue next 
Eg:		fruits = ["apple", "banana", "cherry"]
			for x in fruits:
			  if x == "banana":
			    continue
			 print(x)
# which displays fruits name in order like
				apple
				cherry

range function 
we can set range to specified number of time the set of sequence to be repeated , as  default which starts with 0 , and increment of 1, and end at specified number
Eg:		for x in range(6):
  				print(x) # which prints 0,1,2,3,4 & 5

we can set range to specified number of time the set of sequence to be repeated and we can set start and end range with increment of 1.
Eg:		for x in range(2, 6):
  				print(x) # which displays 2,3,4 & 5

If we want to specify the increment  range
Eg:		for x in range(2, 30, 3):
  				print(x)#which prints 2,5,8,11,14,17,20,23,26 &29.
 		
else in for loop  - like in if statement and for loop,we can use else statement if the for loop condition is false
Eg:		for x in range(6):
  				print(x)
			else:
				print("Finally finished!")	
			#which displays
				0 
				1
				2
				3
				4
				5
			Finally finished!

Nested If - If we want to execute two for loop statement or for loop statement is under another for loop statement,The "inner loop" will be executed one time for each iteration of the "outer loop"
Eg:		adj = ["red", "big", "tasty"]
			fruits = ["apple", "banana", "cherry"]
			for x in adj:
			  for y in fruits:
			    print(x, y)
			#which prints
				red apple
				red banana
				red cherry
				big apple
				big banana
				big cherry
				tasty apple
				tasty banana
				tasty cherry

 Pass -  like in if statement, if there is no content in for loop statement because of some reason and to avoid getting error message. we can type pass.
Eg: 			for x in [0, 1, 2]:
				  pass


Eg:			a = 33
				b = 200
				if b > a:
				  pass