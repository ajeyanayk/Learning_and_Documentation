Bash is a command language interpreter. It is widely available on various operating systems and is a default command interpreter on mst GNU/Linux systems.

**Cat  /etc/shells** - to check which are all shells are available in System.

**Which bash** - to check location of bash shell

**touch filename.sh** - to create a shell file

At the beginning of the bash script need to use
#! bash location - to get know the file is bash file
'Eg : #! /bin/bash'
'where /bin/bash - bash location'

 './filename.sh - to execute the shell file'

**Chmod  xxx filename.sh** - to change the file and x is permission to be allocated to the file
'Eg : chmod 777 file1.sh'

We can give comments using  "#" while coding
	Eg: # this is just a name


Variable Store the date like String number etc

There are 2 types of variable 

1.**System Variable** --> Which are defined by System or predefined
'Eg: echo $BASH' - to display the path of the bash shell location
      'echo $BASH_VERSION' - to display the bash shell version
these variable are defined in Capital Leters

2.**User Defined Variable** - Which are defined by User while  coding
'Eg: X =10',  Here Variable should not start with Numbers 

**Read User Input - Input from Keyboard & assigned to variable**
'Eg: echo "Enter Name :  "'
read name 
echo " Entered Name $name"
If input to to typed in the same line
'Syntax : read -p "    "      Variable
Eg:  read -p " Entername :  " name'

If Input should not be displayed while typing
'Syntax : read -sp " password :    "  password
Eg: read -sp " password :      "  password'

If variable is array 
Syntax : read -a variable
'Eg: echo "Enter name:   "'
read -a name

If the input is multiple  names
**Syntax : read -a **
'ech0 " names : {name[0]},{name[1]} "'

If variable is not mentioned
**Syntax : read**
'Eg: echo  " Enter value : "'
read
echo " value :$REPLY" 
where REPLY is the default variable.

**Pass Argument to Bash Script**

echo $1 $2 $3 
whenever we passed the argument from bash script, they are stored in predefined variable like 1,2,3 
'Eg: echo $1,$2,$3  > echo $1 $2 $3'

If the argument is array
**Syntax : args = ("$@")**
where @ stores argument as array
Argument should be passed while executing shell script.
'Synatx : ./file1.sh arguments
Eg: ./hello.sh  ajeya vijay ram'

If we want to number of arguments passed 
we can use # as variable
'Eg: echo #, which displays the number of argument passed.'

**If then Statement
'syntax : if [condition]
then 
statement
fi'

**If then else statement**
'Syntax : if [condition]
then 
statement 1
else
statement 2
fi'

**If then elif else**
'Syntax : if [condition 1]
then 
statement 1
elif [condition2]
then 
statement 2
else
statement 3
fi'

**File Test Operator**
'Eg: echo -e "Enter the file : \C"'
read filename
'if [-e $filename ]
then 
statement 1
else 
statement 2
fi
Where -e flag - check the file existence'

Similarly
Flag	| Meaning
--------|--------------------------
-f flag | to check file is regular
--------|--------------------------
-d flag |  to check directory
--------|--------------------------
-c flag |  to check the file is character special ( text, data etc.)
--------|--------------------------
-b flag | to check the file is block special (binary, image,music file etc.)
--------|--------------------------
-s flag | to check file is empty
--------|--------------------------
-r flag | to check the file has read permission
--------|--------------------------
-w flag | to check the file has write permission
--------|--------------------------
-x flag | to check the file has the permission to execute.
--------|--------------------------

**head** command to display n number of line or charecters  in file
for example

if we want to print first 20 lines
then
'head -20'

if we want to print first 30 words
then 
'head -c20'

**tail** command to display n number of line or charecters in file
for example 
if we want to print n number of lines from 13 number
then 
'tail -n +13'

if we want to print to last 30 number of lines
then
'tail -n -30'

if we want to print to last 20 charecters in file
then
'tail -c 20'

**tr** - command to replace  charecter with another  charecter
if we want to replace () with []
'tr "()" "[]"'

**tr -d** command to replace delete charecter 
**tr -d a-z**   - which will delete lower case alphabets

**tr -s**
if we want to delete  two spaces to one space 


**Uniq** - which we delete the duplicate values from files