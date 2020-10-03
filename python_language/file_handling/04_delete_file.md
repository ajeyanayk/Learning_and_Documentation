# Deleting File in Python

* To delete file, we need to import OS module  and run **os.remove()** function <br />
	*Eg*: ```import os``` <br />
		  ```os.remove("demofile.txt")``` 

* Check whether file exists or not (to avoid error message, we can check the existence of file before deleting file). <br />
	*Eg*: ```import os``` <br />
		  ```if os.path.exists("demofile.txt"):``` <br />
		  	```os.remove("demofile.txt")``` <br />
		  ```else:``` <br />
		  	```print("The file does not exist")``` 

**Delete folder**
	
+ If we want delete  folder,we can use **os.rmdir()**, but the folder should be empty <br />
	*Eg*: ```import os``` <br />
		  ```os.rmdir("myfolder")```
