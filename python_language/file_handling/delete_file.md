To delete file, we need to import OS module  and run os.remove() function
Eg:	import os
		os.remove("demofile.txt")

Check whether file exists or not
	To avoid error message, we can check the existence of file before deleting file.
Eg:	import os
		if os.path.exists("demofile.txt"):
		  os.remove("demofile.txt")
		else:
		  print("The file does not exist")

Delete folder
	If we want delete  folder,we can use os.rmdir() method and the folder should be empty
Eg:		import os
			os.rmdir("myfolder")
