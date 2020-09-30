In while loop, we can execute the set of statement till the condition is true
Eg:		i = 1
			while i < 6:
  			print(i) # which execute the number from 1 to 5
  			i += 1

The break statement - in this statement we can stop the loop even though the statement is true. 
Eg:		i = 1
			while i < 6:
				print(i)
			if i == 3:
		    	break
			i += 1 # which displays only 1 ,2 & 3

 The continue statement -  in this statement , we can stop the iteration and continue with next
Eg:		i = 0
			while i < 6:
				i += 1
			if i == 3:
				continue
			  print(i) # which displays only 1 ,2,4,5 & 6

else statement - like if statement, we can use else statement if while condition is false
Eg:			i = 1
				while i < 6:
  					print(i)
  					i += 1
				else:
	 				print("i is no longer less than 6")