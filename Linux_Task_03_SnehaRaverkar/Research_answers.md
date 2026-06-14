# PART A :-
1. What is a Process?   
Ans:-A process is a program that is currently running on the computer. Every application or command that is executed creates a process.

2. What is a PID?
 PID stands for Process ID. It is a unique number assigned by the operating system to identify each running process.

3. Which process is consuming the most CPU?
 The process consuming the most CPU is firefox-esr with 0.3% CPU usage.
 
4. Which process is consuming the most Memory?  
The process with the highest value is consuming the most memory.firefox-esr with 22.3% memory usage. Is the process consuming the most memory.


# PART D

## 1.What is a Service?
A service is a program that runs in the background and performs specific tasks for the operating system or users. Services usually start automatically when the system boots.

## 2.Why are Services Important?
Services are important because they provide essential functions such as networking, remote access, printing, and system management. Many system operations depend on services running correctly.

## 3.How Can a Stopped Service Affect a System?
If an important service stops running, related system functions may stop working. For example, if the NetworkManager service is stopped, network connectivity may be affected. Similarly, if the SSH service is stopped, remote access to the system may not be available.

# Part F

# Linux Networking and User Monitoring Commands

## 1. netstat

### Purpose

`netstat` is used to display network connections, routing tables, interface statistics, and listening ports.

### Example Output

```bash
tcp   0   0 0.0.0.0:22   0.0.0.0:*   LISTEN
```

### Security Use Case

Security professionals use `netstat` to identify open ports and active network connections that may indicate unauthorized access or suspicious activity.

---

## 2. ss

### Purpose

`ss` is used to display socket statistics and active network connections. It is a faster replacement for `netstat`.

### Example Output

```bash
tcp   LISTEN   0   128   0.0.0.0:22   0.0.0.0:*
```

### Security Use Case

It helps security analysts monitor open ports, active connections, and network services running on a system.

---

## 3. who

### Purpose

`who` displays information about users currently logged into the system.

### Example Output

```bash
sneha  pts/0  2026-06-14 08:30
```

### Security Use Case

Administrators can verify who is currently logged in and detect unauthorized user sessions.

---

## 4. w

### Purpose

`w` shows information about logged-in users and their current activities.

### Example Output

```bash
USER   TTY   LOGIN@   IDLE   JCPU   PCPU   WHAT
sneha  pts/0 08:30    1:00   0.05s  0.02s  bash
```

### Security Use Case

It helps monitor user activity and identify suspicious or unexpected processes being run by users.

---

## 5. last

### Purpose

`last` displays the login history of users on the system.

### Example Output

```bash
sneha  pts/0  192.168.1.10  Sun Jun 14 08:30
```

### Security Use Case

Security teams use `last` to review login history, investigate unauthorized access attempts, and perform forensic analysis after security incidents.

