# cp and mv command
**cp** - The command used to copy files and directories. 
Syntax :  ```cp option [source] [destination]```

* (If source is a file and destination is not exist currently, Then this command will create the destination file and copy the content of the file.)
Please note, here source may be several but destination should be one.

_Eg: cp [source1][source2][destination]_

* If we want to copy the file to directory, then we can use 
Syntax :``` cp [source file][destination directory]```

* If we want to copy the file to directory and file is already exists in the same name,  the we need to use the flag -i to avoid over-right as it will ask before over-right we need to give yes(y) no (n) before proceeding.

* If we want to copy the directory (which has file) to directory, then
* If the destination directory already exist, then the source directory will copied to destination directory. It literally means the source directory will inside the destination directory.
* If the destination directory doesn't exist, then the command will not create a new directory and which omit an error. To overcome from this error, we need to use flag -R (Recursive) and then the file inside the source directory will be copied to destination directory. Here only file inside source directory will be copied.
Syntax : ```cp -R [source directory] [destination directory]```
(If we destination is current directory we can "." instead of full destination path)

**mv** - move command, this command can be used to move the directory from source to destination.
Syntax : ```mv [option] [source] [destination]```

Please note, here source may be several but destination should be one.
* If the destination directory already exist, then the source directory will moved to destination directory. It literally means the source directory will be moved to destination directory.
If the destination is doesn't exist currently the command will create destination directory or files and then move.  