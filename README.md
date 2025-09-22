Operating Systems Lab Assignment 1
Topic: Process Creation and Management Using Python OS Module
Course Details
Course Code & Name: ENCS351 Operating System
Program: B.Tech CSE "CORE"

Project Overview
This project simulates Linux process management using Python. It replicates key operating system behaviors such as process creation, command execution, zombie/orphan process scenarios, process inspection via /proc, and process prioritization with nice values.

Assignment Objectives
Understand Linux process lifecycle and management.
Create child processes and execute system commands programmatically.
Simulate and observe zombie and orphan processes.
Inspect and extract process information from the /proc filesystem.
Demonstrate the impact of process priority on scheduling.
Tasks Implemented
Process Creation Utility
Creates N child processes using os.fork(). Each child prints its PID and parent PID, followed by a custom message. The parent waits for all children to finish.

Command Execution Using exec()
Modifies task 1 so each child executes Linux commands such as ls, date, or ps using os.execvp().

Zombie and Orphan Processes Simulation
Demonstrates zombie processes by skipping wait() in the parent and orphan processes by exiting the parent before child termination.

Process Inspection from /proc
Takes a PID input and displays process status, executable path, and open file descriptors by reading /proc/[pid]/ files.

Process Prioritization Using Nice Values
Launches multiple CPU-intensive child processes with varying nice values and observes the order of execution influenced by process priority.

How to Run
Ensure you are on a Linux system with Python 3 installed. The script uses Linux-specific modules and filesystem paths.
Clone or download the repository and navigate into the project directory.
Run the Python script:
For Task 4, provide a valid PID when prompted, or press Enter to skip.
For Task 3, observe zombie processes from another terminal by running:
The script outputs messages for each task indicating process creation, command execution, and task completion.
Karan Lal Shah
2301010418
B.Tech Computer Science Engineering (Section : G) K.R. Mangalam University
