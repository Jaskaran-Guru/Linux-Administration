Experiment 6  -- >  File and directory manipulation (cp, mv, rm, mkdir, rmdir) 

File and Directory Manipulation in Ubuntu

Managing files and directories in Ubuntu using the terminal is essential for efficient workflow. The following commands help in copying, moving, renaming, deleting, and creating files and directories.

1. Copying Files and Directories (cp)

A. Copying a File

The cp command copies files from one location to another.

**cp source.txt destination.txt**

![image](https://github.com/user-attachments/assets/1b979179-4ee9-4a46-a596-77b26c620f37)

B. Copying a File to Another Directory

**cp file.txt /home/jaskaran/Documents/**

![image](https://github.com/user-attachments/assets/355ac6a2-63c7-4de3-9438-9d877a845331)


C. Copying a Directory (Recursive Copy)

Use the -r flag to copy directories.

**cp -r my_folder /home/jaskaran/backup/**

![image](https://github.com/user-attachments/assets/9eee6468-d97b-4851-87e6-b5eeb7fb0f75)



2. Moving and Renaming Files (mv)

A. Moving a File to Another Location

**mv file.txt /home/jaskaran/Documents/**

![image](https://github.com/user-attachments/assets/85d2b022-1e92-4081-ba60-9a2201a8c474)

Ḃ. Renaming a File

**mv oldname.txt newname.txt**

![image](https://github.com/user-attachments/assets/37e71a86-ae7e-4495-8658-f850d89fc2de)


C. Moving a Directory

**mv my_folder /home/jaskaran/backup/**


4. Deleting Files and Directories (rm)

A. Removing a File

**rm file.txt**

![image](https://github.com/user-attachments/assets/22e639e5-ddcc-4c2e-a2e6-c9789506f04f)


B. Removing Multiple Files

**rm file1.txt file2.txt file3.txt**

C. Removing a Directory (Recursively)

Use the -r option to delete a directory and its contents.

**rm -r my_folder**

D. Force Deleting a Directory

The -f flag forces deletion without confirmation.

**rm -rf my_folder**
![image](https://github.com/user-attachments/assets/f3408dcd-5048-40c2-81ce-ae1909680883)



⚠️ Be careful with rm -rf, as it can permanently delete important files!

5. Creating Directories (mkdir)

A. Creating a Single Directory

**mkdir my_folder**

B. Creating Multiple Directories

mkdir project1 project2 project3



