Experiment 8  --> Basic process management (ps, top, kill) 

Process management in Linux is crucial for monitoring and controlling running tasks. The key commands are:

ps → View processes
top → Monitor system resources and processes
kill → Terminate processes

1. Viewing Processes (ps)

The ps command displays running processes.

A. Show Active Processes

ps
Displays processes started in the current shell.
B. View All Processes (ps aux)

ps aux
a → Show processes of all users
u → Display user details
x → Show system processes
C. Filter by Process Name

ps aux | grep firefox
This finds all firefox processes.
D. Show Processes in a Tree Format

ps -ef --forest
Displays parent-child process relationships.
2. Monitoring System Resources (top)
The top command provides a real-time view of processes and system usage.

A. Start top

top
Shows CPU, memory, and running processes.
B. Common Shortcuts in top
Key	Action
q	Quit
k	Kill a process (enter PID)
r	Renice (change process priority)
Shift + M	Sort by memory usage
Shift + P	Sort by CPU usage
C. Use htop (Better Alternative to top)
Install htop for an interactive interface:


sudo apt install htop
htop
3. Killing Processes (kill)
The kill command terminates processes using their Process ID (PID).

A. Find the Process ID (PID)

ps aux | grep firefox
The second column shows the PID.
B. Kill a Process by PID

kill 1234
Replace 1234 with the actual PID.
C. Force Kill a Process

kill -9 1234
The -9 option forcefully terminates the process.
D. Kill a Process by Name (pkill)

pkill firefox
This kills all firefox processes.
E. Kill All Processes by Name (killall)

killall firefox
Terminates all firefox instances.
