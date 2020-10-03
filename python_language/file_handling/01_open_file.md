# File Handling in Python  - Introduction

***Python has several functions for creating, reading, updating and deleting file***.

+ **Open a file** : to open a file or working with files, we need to use open() function and  open() function takes parameter - filename and mode <br />
	Syntax:	```f = open("demofile.txt", "rt")```<br />
		       *The code above is the same as:* <br />
		      ```f = open("demofile.txt")``` *"r" for read, and "t" for text are the default values.*

#### There are four different modes for opening file,

| **Key** | **Mode** | **Description |
|---------|---------|------------|
| "r" | Read | Default value. Opens a file for reading, error if the file does not exist |
| "a" | Append | Opens a file for appending, creates the file if it does not exist |
| "w" | Write | Opens a file for writing, creates the file if it does not exist |
| "x" | Create | Creates the specified file, returns an error if the file exists |

**Depending on the file, additionally we have 2 more mode** <br />
* "t" - Text - Default value. Text mode <br />
* "b" - Binary - Binary mode (e.g. images)




 