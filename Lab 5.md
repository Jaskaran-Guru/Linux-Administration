Experiment 5 -->   Basic Command Line Skills: Introduction to  the terminal and shell (bash shell in  Ubuntu), Navigating the file system (ls, cd,  pwd, and Ubuntu directory structure)

Basic Command Line Skills in Ubuntu
The Linux terminal (or command line) is a powerful tool for managing the operating system efficiently. Ubuntu primarily uses the Bash shell (Bourne Again Shell) as its default command-line interface.

1. Introduction to the Terminal and Shell
   

What is a Shell?

A shell is a command-line interface that allows users to interact with the operating system.
Ubuntu uses Bash (Bourne Again Shell) by default, but others like Zsh, Fish, and Dash are also available.

How to Open the Terminal?

Keyboard Shortcut: Press Ctrl + Alt + T.
From Applications: Search for "Terminal" in the application menu.
In a Virtual Console: Press Ctrl + Alt + F3 (To switch back to GUI, use Ctrl + Alt + F2).

3. Navigating the File System

A. Checking the Current Directory (pwd)

The pwd (print working directory) command shows your current location in the file system.

**pwd**
![image](https://github.com/user-attachments/assets/3a7876a5-9228-45c7-8110-d5c874fe8f50)


B. Listing Files and Directories (ls)

The ls command lists files and directories in the current location.

ls
![image](https://github.com/user-attachments/assets/a065cf01-9bab-4608-9383-7605529d6114)


Useful Options:

Command	Description
ls -l	Lists files with details (permissions, owner, size, date)
ls -a	Shows hidden files (files starting with .)
ls -lh	Lists files in human-readable sizes (KB, MB)

C. Changing Directories (cd)

cd (change directory) moves between directories.

![image](https://github.com/user-attachments/assets/1522d235-f02d-45f1-8ea3-78940d9cd3ed)



Common cd Commands:
Command	Description
cd /	Go to the root directory
cd ~	Go to the home directory (/home/username)
cd ..	Move one directory up
cd -	Switch to the last directory

D. Ubuntu Directory Structure

Linux follows a structured directory system. Important directories include:

Directory	Purpose
/	Root directory (contains all other directories)
/home/	Stores personal user files (/home/jaskaran)
/bin/	Essential system binaries (commands like ls, cp)
/etc/	System configuration files
/var/	Logs and variable data
/tmp/	Temporary files (cleared on reboot)
/usr/	User-installed applications
/mnt/	Mounted file systems (external drives)
