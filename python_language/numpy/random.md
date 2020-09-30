Random - Random numbers are those that cannot be predicted. 
Pseudo Random - If the numbers are generated through a generation algorithm 
Truly Random - If the numbers are generated through any generation algorithm or predicted logically.

We are working on Pseudo random numbers

Generate Random Number - we need to Random function from Numpy module to work with Random Number
Eg:		#Generate a random integer from 0 to 100
			from numpy import random
			x = random.randint(100) # to generate random integer we need to use randint()

			print(x) # Eg. 5

Generate Random Float - to generate random float number, we need to use rand()
Eg:		#Generate a random integer from 0 to 100
			from numpy import random
			x = random.rand()

			print(x) # Eg. 12.0

Generate Random Array - 
we can create Random Array with Integer value, Then we need to use randint() and need to mention the size. 

Eg 1:		from numpy import random
			x=random.randint(100, size=(5))

			print(x) # Eg. [15,56,58,42]

Eg 2:	from numpy import random
			x = random.randint(100, size=(3, 5))# Here 3 is row and 5 is size

			print(x)
			#it may display
		[[90 99 11 30 34] 
        [66 40 63 36 37] 
        [63 35 89 51 58]]


similarly if want float value then we need to use rand() with mention size .
Eg 1:		from numpy import random
			x = random.rand(5)

			print(x) #[0.1987822 0.8190278 0.7456011 0.1469775 0.3002084]

Eg 2 :	from numpy import random
			x = random.rand(3, 5)

			print(x)
      [[0.14252791 0.44691071 0.59274288 0.73873487 0.22082345] 
       [0.00484242 0.36294206 0.88507594 0.56948479 0.15075563] 
       [0.69195833 0.75111379 0.92780785 0.57986471 0.6203633 ]]

Generate Random Number from Array -  If we  require a random number from set of an array, we can use 
Eg:		from numpy import random
			x = random.choice([3, 5, 7, 9])

			print(x)

  If we want to make array/s we can use choice and also mention size to specify the size of the array
Eg:	#Generate a 2-D array that consists of the values in the array parameter (3, 5, 7, and 9)
			from numpy import random
			x = random.choice([3, 5, 7, 9], size=(3, 5))

			print(x)
Eg:		[[9 3 5 5 7] 
         [7 5 3 3 9] 
         [7 5 9 9 7]]
