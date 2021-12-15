# What is VIM
* Vim is  not included in Ubuntu
* To install vim
  * Sudo apt install vim
  
  Vim has insert modes
   -i 
  
• if vi is installed in all Linux distros, Why am i learning VIM?
vim has more features
vim is easier to learn
vim is also very light weight
most vim commands are backwards compatible with vim

## How to start and quit Vim?
• To start vim type vim. The text editor will start in normal mode.
• To quit vim press esc and type :ga!
g
a
-D
prefix for entering command line mode
-5
short for quit
short for all buffers
-.
force
quit all now
• To set line numbers: set number

## Vim modes:
• Insert mode: used for writing text
Normal mode: used for manipulating text
Command mode: used for entering vim commands
Visual mode: used for navigation and manipulation of text selections
Select mode: similar to visual mode
Ex-mode: Similar to the command-line mode but optimized for batch
processing.
When you start vim, you are in normal mode
From normal mode press i to enter insert mode
The word -INSERT- will appear on the bottom left corner of the terminal indicating that you are in insert mode
To switch back to normal mode press esc
In the lack of the esc key press ctrl +


## Insert text:
You can create a file and open vim at the same time by typing vim and a
file name.
Example:
vim notes. txt
In insert mode, you can use:
The arrow keys to move around,
Enter Key to continue in the next line,
Backspace for deleting

## Install vim
sudo apt install vim
-Y
Start vim
2
vim
Enter insert mode
Press letter i
Enter normal mode
2
Press esc key
Quit vim
Type :g!
Start vim
vim
Enter insert mode
Press letter i
Type 3 sentences
I like linux.
Pizza is great.
I go to school.
Exit vim without saving
Press esc key
Type :g!


## Saving and quitting vim
Terminsl
Helo
To save a text file you need to
enter normal mode using : and the
use the w key
File
Edit
View
an a tilel
Terminal
Tabr I
will save the file w new. txt
will save the file as new.txt + wa
will save the file and quit + wqa 
will save the file and close all
files open in the buffer