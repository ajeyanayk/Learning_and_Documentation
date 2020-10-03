# Reading a File in Python

+ If a file in same folder as Python and want read the content of the file, we can use the **read()** method.
	*Eg*:	```f = open("demofile.txt", "r")``` **open()** *is must to perform any kind activity on file*
			```print(f.read())```

+ If the file located in a different location, we need to specify the location
	*Eg*:	```f = open("D:\\myfiles\welcome.txt", "r")``` *If the file is in* **D:\\myfiles\welcome.txt**
			```print(f.read())```

+ If we want to read specified number of character
	*Eg*:	```f = open("demofile.txt", "r")```
			```print(f.read(5))``` *it returns 5 character from demofile.txt*

    *Read Lines - if we want to read the file line wise, we can use* **readline()** *method,*

+ If we want to display first 2 lines. we need to call **readline()** twice.
	*Eg 1*: ```f = open("demofile.txt", "r")```
			```print(f.readline())``` *which displays first line of the content*

	*Eg 2*: ```f = open("demofile.txt", "r")```
			```print(f.readline())``` *which displays first line of the file*
			```print(f.readline())``` *which displays second line of the file*

    We can also read the file by looping method
	*Eg*:	```f = open("demofile.txt", "r")```
			```for x in f:```
			  ```print(x)```

+ **Close file** - we can close the file using close() method
	*Eg*:	```f = open("demofile.txt", "r")```
			```print(f.readline())```
			```f.close()```

*We should always close your files, in some cases, due to buffering, changes made to a file may not show until we close the file*.



