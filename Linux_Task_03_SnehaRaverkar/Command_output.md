# Part A: Process Monitoring
## 1. ps
Shows the processes running in the current terminal session along with their PID, terminal, CPU time, and command name.

## 2. ps aux
Displays detailed information about all running processes, including the user, PID, CPU usage, memory usage, and command.

## 3. top
Shows real-time system performance information such as CPU usage, memory usage, and the list of running processes.

## 4. htop
Provides an interactive and user-friendly view of system processes, CPU usage, memory usage, and process details.

# Part B:

## ps aux | grep sleep: 

sneha      19077  0.0  0.1   5616  2100 pts/2    SN   07:20   0:00 sleep 300

sneha      19883  0.0  0.1   5616  2172 pts/2    SN   07:22   0:00 sleep 300

## kill 19077:
This kills the process
