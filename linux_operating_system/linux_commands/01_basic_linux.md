# Basic Linux Commands
**pwd** - Present Working Directory, which shows current working directory which we are current working in.
Syntax : ```pwd```

**Redirection (>)*** - It means capturing output from file, command or programs and send it as input to another file, command or program.
Syntax : ```cat  > [filename 1]```

* (If we don't have any text file with same name, it generate the text file automatically. If we are already using any text file it overwrites and update with new contents)
where  > redirection symbol which we are used  transfer the output  to file (which given in command after >).

* If we want update the currently working file and then we use >, It overwrites existing contents. To overcome this problem we need to use >> (If we want to update the file without damaging the current  details). We need to use the command ```cat >> [file name]```

* If we want to add the  two files and move it to another file we can use the ```cat [file 1] [file2] >[file3]```
* Similarly if we want to move file 1 data directly to file 2  then we can use  ```cat [file 1]  >> [file 2]```
Please note, We can use the redirection  whenever we want to update the result to new file.

**man** - Which shows the details and option of corresponding commands 
Syntax : ```man command name```

_Eg: man ls_
where ls is list command which shows the content of the files. When we type ls command after man we can get the option and combination of ls.
Once we see the details of command we need to press **clt+q** to come back to terminal.