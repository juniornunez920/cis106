
# Lecture 3    

In Linux you will hear directory many times. Directory is also known as "folder"

# Navigating the FS in the CLI 
## The Linux Directory Structure
- Think of the file system as a tree where every branch represents a directory (folder)
- You are always working insde a particular directory and you can move forward to a subdirectory
- The directory where you are at the moment is called the current working directory or present working directory 
- In a filesystem, every file has a pathname which indicates the location of the file in the filesystem (like an address).

The file structure always starts at the root '/'. It follows the sub-folders to create a pathname until it reaches the file in search of. 

#ALWAYS USE ABSOLUTE PATH
The path might be long 

Relative path 

A few commands 
<b>* The pwd command- </b> used for displaying the current working directory 
* The cd command - used for changing 
directory
What it does? 
The working directory is represent by a Single dot or 2 dots. 

commands 
cd takes you home 
cd ~ takes you home as well (~ = home$ User)
cd $HOME


~ short hand for home directory 
Home directory 
/home/student | $HOME/student | Home directory 











* The ls command - used for displaying all the files inside a given directory. Whne no directory is specified, ls displays the files in the current working directory. 
  ## Types of pathnames: 
<b>*  Absolute path - States the full pathname starting from root (/). Always starts from the root</b>
*  Example: /home/juniornunez920/Downloads/egypt.mp3

<b>*  Relative Path - Specifies the pathname starting from the current directory. Always starts with a subdirectory.</b>
-  Example: Downloads/egypt.mp3






Sources https://github.com/ra559/cis106