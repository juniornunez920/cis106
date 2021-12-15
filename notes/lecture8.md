# Lecture 8 
### 12/01/21

## Shell Scripting (Intro)


###  
## Before you start shell scripting it is important that you understand the following concepts:
#### Source code vs machine code:
#### Source code is the human readable code written in a programming language like Python. machine code consists of binary 1s and Os and is the language a computer's CPU understands.

### Compiler: a program used for converting a complete source code into machine code.Interpreter: a program that converts source code into machine code line by line. Compiled program vs Interpreted program:a compiled program is a binary file produced by a compiler. an interpreted program is a program that requires an interpreter to interpret and run each Shell scripts are examples of interpreted programs, and the interpreter used is the BASH shell. Creating a shell script is as simple as creating a file and then assigning execute permission for it. After creating a shell script and assigning execute permission, you must enter the absolute or relative path to where it's stored to run it.

#### To Dipslay a line of text use the echo command: Example
### echo "This is a message" 
### echo "This is another message" "and another message"
#### echo -n "this is , again another message"

## Working with variables

# Variable: placeholder for data.
## Environment variable; is a placeholder for data that can change; typically, it gets its value automatically from the OS startup or the shell being used. Each user has environment variables with  different values to define his or her working environment. The HOME environment variable stores the absolute pathname to a user's home directory, so it varies for each user. Some environment variables are the same for all users logged in to a machine, such as the HOST environment variable that specifies the computer name. The env command allows you to see all environment variables You can use the echo command to see the value of an environment variable. 1 Example:
### • echo SHOME
### • echo $HOST

####  Practice: Type vim script2.sh, enable line numbers, and enter insert mode.
#### Type:
#### * #!/bin/bash  computer="office-computer" echo "What is your name:"                                  read name                                echo "Hello, $name you are in $computer" Save your file and close vim             Make the file executable with: chmod u+ script2.sh                                Run the script with: ./script2.sh