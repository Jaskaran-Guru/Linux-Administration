Experiment 7 --> Basic Command Line Skills: Viewing and  editing files (cat, less, head, tail, nano, vim)

1. Viewing Files

A. Displaying File Contents (cat)

The cat command prints the entire content of a file.

**cat filename.txt**

Combine multiple files and display their content:

**cat file1.txt file2.txt**

B. Viewing Files Page-by-Page (less)

The less command allows scrolling through large files.

less filename.txt

Navigation inside less:
↑ / ↓ → Scroll line by line
Space → Move down one page
b → Move up one page
q → Exit

C. Viewing theFirst Few Lines of a File (head)

Displays the first 10 lines of a file by default.

**head filename.txt**

Show a specific number of lines (e.g., first 5 lines):

**head -5 filename.txt**

D. Viewing the Last Few Lines of a File (tail)

Displays the last 10 lines of a file by default.

tail filename.txt
Show the last 5 lines:

**tail -5 filename.txt**

Continuously monitor a file (useful for logs):

tail -f /var/log/syslog

3. Editing Files

A. Editing with Nano (nano)

Nano is a beginner-friendly text editor.

Open a file in nano:

**nano filename.txt**

Basic Commands in Nano:

Command	Action
Ctrl + X	Exit
Ctrl + S	Save file
Ctrl + O	Save as (Write file)
Ctrl + W	Search text
Ctrl + K	Cut a line
Ctrl + U	Paste a line

**nano newfile.txt**

B. Editing with Vim (vim)

Vim is a powerful, advanced text editor.

Open a file in Vim:

**vim filename.txt**

Basic Vim Modes:
Mode	Description
Normal Mode	Press Esc to navigate
Insert Mode	Press i to insert text
Command Mode	Press : to execute commands
Basic Vim Commands:
Command	Action
i	Insert text
Esc	Exit insert mode
:w	Save the file
:q	Exit Vim
:wq	Save and exit
:q!	Exit without saving
Example: Open a file, edit, and save

**vim myfile.txt**

Press i to enter Insert mode.
Type text.
Press Esc, then type :wq and press Enter.


Screenshots  for  the above  commands :

![image](https://github.com/user-attachments/assets/5bf43c02-7912-4e4b-861f-43f8bff43ca2)
