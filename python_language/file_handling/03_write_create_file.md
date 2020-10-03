# Write a File in Python

**Writing existing file** - to write to existing file, we need to use any one of the following parameter in open() function,

| **Key** | **Mode** | **Description |
|---------|---------|------------|
|"a" | Append | will append to the end of the file|
|"w" | Write | will overwrite any existing content|

*Eg 1* : ```f = open("demofile2.txt", "a")``` <br />
		 ```f.write("Now the file has more content!")``` *will append existing file content* <br />
		 ```f.close()``` <br />
		 *open and read the file after the appending* <br />
		 ```f = open("demofile2.txt", "r")``` <br />
		 ```print(f.read())```

*Eg 2* : ```f = open("demofile3.txt", "w")``` <br />
		 ```f.write("Woops! I have deleted the content!")``` *content get overwrite in existing file* <br />
		 ```f.close()``` <br />
		 *open and read the file after the appending* <br />
		 ```f = open("demofile3.txt", "r")``` <br />
		 ```print(f.read())``` <br />

+ **Creating a New File** : to create a new file, we need to use open() with one of the following parameter,

| **Key** | **Mode** | **Description |
|---------|---------|------------|
|"x" | Create | will create a file, returns an error if the file exist|
|"a" | Append | will create a file if the specified file does not exist|
|"w" | Write  | will create a file if the specified file does not exist|

*Eg*: ```f = open("myfile.txt", "x")``` **new empty file is created!**

+ If we want to create and write the file together: <br />
	*Eg*: ```f = open("myfile.txt", "w")```