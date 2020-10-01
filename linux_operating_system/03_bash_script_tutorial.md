# Bash Script Tutorial

### Bash is a command language interpreter. It is widely available on various operating systems and is a default command interpreter on mst GNU/Linux systems.

**Cat  /etc/shells** - to check which are all shells are available in System. <br />
**Which bash** - to check location of bash shell <br />
**touch filename.sh** - to create a shell file <br />

At the beginning of the bash script need to use
#! bash location - to get know the file is bash file <br />
_Eg_ : ```#! /bin/bash``` <br />
```where /bin/bash``` - bash location <br />
```./filename.sh ```- to execute the shell file <br />

**Chmod  xxx filename.sh** - to change the file and x is permission to be allocated to the file <br />
_Eg_ : ```chmod 777 file1.sh```

We can give comments using  "#" while coding <br />	
_Eg_: # this is just a name_

### Variable Store the date like String number etc <br />

#### There are two types of variable 

+ **System Variable** --> Which are defined by System or predefined <br />
	* ```echo $BASH``` - to display the path of the bash shell location <br />
  * ```echo $BASH_VERSION``` - to display the bash shell version _These variable are defined in Capital Leters_

+ **User Defined Variable** - Which are defined by User while  coding <br />
_Eg_: X =10_,  Here Variable should not start with Numbers 

**Read User Input - Input from Keyboard & assigned to variable** <br />
_Eg_: ```echo "Enter Name :  "``` <br />
        read name 

```echo " Entered Name $name"``` <br />
* If input to to typed in the same line

Syntax : ```read -p "    "      Variable``` <br />
_Eg_:  ```read -p " Entername :  " name'``` 

* If Input should not be displayed while typing <br />
Syntax : ```read -sp " password :    "  password``` <br />
_Eg_: ```read -sp " password :      "  password`` `

* If variable is array  <br />
  Syntax : ```read -a variable``` <br />
_Eg_: echo "Enter name:   "_ <br />
```read -a name```

* If the input is multiple  names

Syntax : ```read -a ```<br />
```ech0 " names : {name[0]},{name[1]} "```

* If variable is not mentioned

Syntax : ```read   ``<br />
_Eg_: ```echo  " Enter value : "```<br />
```read```

```echo " value :$REPLY" ```<br />
where REPLY is the default variable.

**Pass Argument to Bash Script**

```echo $1 $2 $3```<br />
whenever we passed the argument from bash script, they are stored in predefined variable like 1,2,3 <br />
_Eg_: ```echo $1,$2,$3  > echo $1 $2 $3```

* If the argument is array

Syntax : ```args = ("$@")**``` <br /> 
where @ stores argument as array

Argument should be passed while executing shell script. <br />
Synatx :``` ./file1.sh arguments```<br />
_Eg_: ```./hello.sh  ajeya vijay ram```

* If we want to number of arguments passed <br />
we can use # as variable <br />
_Eg_: ```echo #```, which displays the number of argument passed. <br />

**If then Statement**
syntax : 
```
if [condition]
then 
statement
fi
```

**If then else statement**

Syntax : 
```
if [condition]
then 
statement 1
else
statement 2
fi
```

**If then elif else**

Syntax : 
```
if [condition 1]
then 
statement 1
elif [condition2]
then 
statement 2
else
statement 3
fi
```

**File Test Operator**

_Eg_: ```echo -e "Enter the file : \C"```<br />
    ```read filename```
 ```  
if [-e $filename ]
then 
statement 1
else 
statement 2
fi
```


Where -e flag - check the file existence'

Similarly
Flag	| Meaning
--------|--------------------------
-f flag | to check file is regular
-d flag |  to check directory
-c flag |  to check the file is character special ( text, data etc.)
-b flag | to check the file is block special (binary, image,music file etc.)
-s flag | to check file is empty
-r flag | to check the file has read permission
-w flag | to check the file has write permission
-x flag | to check the file has the permission to execute.

**head** command to display n number of line or charecters  in file

for example
* if we want to print first 20 lines <br />
then```head -20```

* if we want to print first 30 words <br />
then ```head -c30```

**tail** command to display n number of line or charecters in file

for example 
* if we want to print n number of lines from 13 number <br />
then ```tail -n +13```

* if we want to print to last 30 number of lines <br />
then ```tail -n -30```

* if we want to print to last 20 charecters in file <br />
then ```tail -c 20```

**tr** - command to replace  charecter with another  charecter
* if we want to replace () with [] <br />
```tr "()" "[]"```

**tr -d** command to replace delete charecter 
**tr -d a-z**   - command to delete lower case alphabets

**tr -s** - command to delete  two spaces to one space 


**Uniq** - command to delete the duplicate values from files