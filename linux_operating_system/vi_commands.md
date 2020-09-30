vi editor stands for Visual editor, which is a text editor and is available on almost Linux / Unix System

We can use the vi editor to edit an existing files or creating an new file or to just read a text file.

There are 2 kind of operating modes in vi editor
 
Command mode :  this mode will enable the user to do administrative task such as saving , editing files, executing the command and moving the cursor. 
Insert mode : this mode enables the user to insert or type the text or command.
 
vi [file name.txt] - to create a text file in terminal 

The vi always start with command mode and for entering a text we need to be in insert mode. 
To come to insert mode we need to press "i" and to quit press "ESC" key.
 If we want to know which mode we are in just press "ESC" button twice . so that you can be in command mode.
Please note, the vi command s are case sensitive. 
    
The following keys perform specific task. we need to press to perform and which is case sensitive. 
Please note to do task we should be in command mode

ZZ (Capital Z)            - to save & quit the file.
Left arrow key or h    - to move the cursor left
Right arrow key or l   - to move the cursor right
Down arrow key or j	- to move the cursor downward
Up arrow or k				- to move the cursor upward
x									- to delete character
dd 								- to delete or cut the line in the file
(If we want to delete or cut multiple lines, then we need to press no.of lines and dd 
Eg : if we want to delete or cut 3 lines , then we need to press 3dd )
p									- to paste 
dw								- to delete or cut the word in the file
(Please note, the command delete from current cursor position  to next word)
yy								- to copy the current line
(If we want to copy multiple lines, then we need to press no.of lines and yy
Eg : if we want to copy 3 lines , then we need to press 3yy )
yw								- to copy the word in the file
(Please note, the command copy from current cursor position  to next word)
/ "word"						- to search a word, "/" is search engine.
n									- to find a word in forward direction
N									- to find a word in backward direction
r									- to change one character at a time
R 								- keep changing character till "ESC" is hit
u									- undo 
Clt+r 							- redo
:w                                - to save the file
:q                                 - to quit
:wq                              - to save & quit (like ZZ)
:ql 								- to force quit (without saving file)