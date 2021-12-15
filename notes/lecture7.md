#Managing US

# Linux File permissions | File Ownership 
A file can be owned only one user 



# Commands 

- The chmod command 

### -  Symbolic Notation 
  ### Managing user accounts involves adding, modifying and deleting user accounts and account's information         To add user accounts we use the useradd or adduser command.
### In Ubuntu, the adduser program is recommended over useradd due to useradd being a low-level utility. To modify user's information we use the ugermod program. To delete a users we use the userdel program.The following files are involved in the user creation process: 

### /etc/login.defs
### /etc/default/useradd
### /etc/skel/
### /etc/passwd
### /etc/shadow
### /etc/group


### How to add user? 
### adduser followed by username 

### To delete 
### userdel -r username 


### The /etc/login.defs file
### It contains directives for use in various shadow password suite commands.Shadow password suite is an umbrella term for commands dealing with account credentials, such as the useradd, userdel, and passwd. The directives (entries or configuration variables) in this configuration file control an array of settings from password length all the way to whether or not a home directory is created when a user is created. The file is typically filled with comments and commented-¡ut directives (which make the directives inactive).Here is an example of how the /etc/login.defs file looks like:
## https://robertalberto.com/cis106/login.defs-file-example.txt
#### Here is how the /etc/login.defs file looks like in your system without any comments:
#### grep -ve ^$ /etc/login.defs | grep -V A#

### PASS_MIN_LENGTH Minimum number of characters required in password.
### PASS_WARN_AGE Number of days a warning is issued to the user prior to a
### password expiration.
### CREATE_HOME Default is no. If set to yes, a user account home directory is
## created.
### ENCRYPT_METHOD The method used to hash account passwords.

# This file stores the system default configuration for creating new users with the, useradd utility.
## To view the default parameters in the /etc/default/useradd file use either of these
## commands:
#### useradd
#### -D
## cat /etc/default/useradd
### If the /etc/login.defs has the directive CREATE_HOME not set or set to no, then the
### users created with the useradd utility will not get a home directory unless the -m
## option is given.
### You can view all the directives as well as what each directive mean in by
### examining the content of the /etc/default/useradd file.
## cat /etc/default/useradd       grep -ve ^$
##  /etc/default/useradd | grep -VAt

# HOME Base directory for user account directories.
## INACTIVE Number of days after a password has expired and has not been changed until the account will be deactivated.
## SHELL User account default shell program. In Ubuntu, this variable is set to /bin/sh which means that after using the useradd command, unless bash is specified, sh will be the default login shell for any user. The /etc/skel/directory The /etc/skel directory stores files that are copied to each user's homedirectory
