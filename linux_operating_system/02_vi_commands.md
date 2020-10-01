# vi editor

### vi editor stands for Visual editor, which is a text editor and is available on almost Linux / Unix System

We can use the vi editor to edit an existing files or creating an new file or to just read a text file.

#### There are 2 kind of operating modes in vi editor
 
* **Command mode** :  this mode will enable the user to do administrative task such as saving , editing files, executing the command and moving the cursor. 
* **Insert mode** : this mode enables the user to insert or type the text or command.
 
**vi [file name.txt]** - to create a text file in terminal 

The vi always start with command mode and for entering a text we need to be in insert mode. 
To come to insert mode we need to press _"i"_ and to quit press _"ESC"_ key.
 
* If we want to know which mode we are in just press _"ESC"_ button twice . so that you can be in command mode.

Please note, the vi command s are case sensitive. 
    
#### The following keys perform specific task. we need to press to perform and is case sensitive. 

| **Sl. No.** | **Keys** | **Performing task** |
----------|--------------|--------------
1|**ZZ** (Capital Z) | to save & quit the file.
2|Left arrow key or **h** | to move the cursor left
3|Right arrow key or **l** |to move the cursor right
4|Down arrow key or **j**  | to move the cursor downward
5|Up arrow or **k**		   |to move the cursor upward
6|**x**					   |to delete character
7|**dd** 				   |to delete or cut the line in the file
8|**p**					   | to paste 
9|**dw**				   |to delete or cut the word in the file (Please note, the command delete from current cursor position  to next word))
10|**yy**					|to copy the current line
11|**yw**				|to copy the word in the file (Please note, the command copy from current cursor position  to next word)
12|**/** "word"						| to search a word, "/" is search engine.
13|**n**							    | to find a word in forward direction
14|**N**								| to find a word in backward direction
15|**r**							| to change one character at a time
16|**R** 								| keep changing character till "ESC" is hit
17|**u**								| undo 
18|**clt+r**							| redo
19|:**q**                             | to quit
20|**:wq**                             | to save & quit (like ZZ)
21|**:ql** 							| to force quit (without saving file)


* If we want to delete or cut multiple lines, then we need to press no.of lines and dd

_Eg : if we want to delete or cut 3 lines , then we need to press 3dd_


* If we want to copy multiple lines, then we need to press no.of lines and yy

_Eg : if we want to copy 3 lines , then we need to press 3yy_






