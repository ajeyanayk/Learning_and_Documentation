# ls commands

**ls** - Linux shell command which lists directory contents  of files and directories
Syntax  : ```ls [Option] [files/directory]```

#### There are few known commands under this category

* ```ls  [No option] [no file name or directory mentioned]```- which list the content of the current working file or directory.
* ```ls [ directory name / path]```- which list the content of the given path in the command
* If we want to list the content in Home file we can use ```** ls ~**```  to get details.
* If we want to know the details of previous file (one step back) of current working directory we can us  ```ls ..```
* If we want to know the content of the previous file (2 step back) of current working directory we can use ```ls ../..```
* ```ls  -l``` - which lists the content of the current working file or directory in detailed manner (long format) , In which we can find the rights , size and date of creation of the files.

** In these there is a column start with - or d which differentiate directory and files. 
** next 9 digit are equally divided in to three parts and which will show the access rights of files, 3 digit shows the access rights  for Owner, Group  and other respectively. 
  Where r denotes read , w  is for write and x for execute. If access right is rwx means the respective controller has full rights ( Read, Write & Execute ), Similary If access right is - - - , Which means controller doesnt have any rights on the corresponding file or directory.
 ls -d ./ - which list the Directoty files in the current working directory.

#### There are also some command which used frequently.
* If we want sort the files by their size.
		Syntax : ```ls  [option] [file/directory path] S```
where file with bigger size which will shown in the first row.

* if we want to check the files details by extention
		Syntax : ```ls  [Files / Directory] [*.ext name]```

* if we want to know directory structure we can use the command
		Syntax : ```ls -R```
which shows the current directory structure.