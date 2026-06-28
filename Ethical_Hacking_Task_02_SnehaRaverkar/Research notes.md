 # PART A:-
Nmap was successfully installed on the system. The installation was verified by executing the following command:
nmap --version

# Part B: Scan Your Local Machine

## Command Used

```bash
nmap localhost
```

## Scan Results

**Total Open Ports:** 3

| Port Number | Service Running |
| ----------- | --------------- |
| 80/tcp      | http            |
| 135/tcp     | msrpc           |
| 445/tcp     | microsoft-ds    |

## Result

The Nmap scan was successfully performed on the local machine (`localhost`). The scan detected **3 open TCP ports**: **80 (HTTP)**, **135 (MSRPC)**, and **445 (Microsoft-DS)**, indicating that these services were active on the local system.


# Part C: Service Version Detection

## Command Used

```bash
nmap -sV localhost
```

## Service Version Detection

| Port Number | Service Name | Version Detected         |
| ----------- | ------------ | ------------------------ |
| 80/tcp      | HTTP         | Microsoft IIS httpd 10.0 |
| 135/tcp     | MSRPC        | Microsoft Windows RPC    |
| 445/tcp     | Microsoft-DS | Version not detected     |

## Result

The `nmap -sV localhost` command was successfully executed on the local machine. Nmap detected the service versions for the HTTP and MSRPC services. The version information for the Microsoft-DS service could not be determined.


# Part D: Operating System Detection

## Command Used

```bash
nmap -O localhost
```

### Was the operating system detected?

**Answer:** Yes

### Which OS was identified?

**Answer:** Microsoft Windows 11 (24H2 – 25H2)

### Why is OS detection useful during penetration testing?

Operating system detection helps penetration testers identify the target operating system. This information is useful for selecting appropriate vulnerability scans, identifying potential security weaknesses, choosing compatible exploits, and planning effective security assessments.

# Part E: Common Port Research

| Port      | Protocol                                   | Purpose                                                                                                                       | Common Security Risks                                                                                             |
| --------- | ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| **20/21** | FTP (File Transfer Protocol)               | Transfers files between a client and a server. Port 20 is used for data transfer, while Port 21 is used for control commands. | Data and passwords are transmitted in plain text, making them vulnerable to interception and brute-force attacks. |
| **22**    | SSH (Secure Shell)                         | Provides secure remote login and encrypted communication between systems.                                                     | Weak passwords, brute-force attacks, and outdated SSH software can lead to unauthorized access.                   |
| **23**    | Telnet                                     | Allows remote login to a computer or network device.                                                                          | Sends all data, including usernames and passwords, in plain text, making it highly insecure.                      |
| **25**    | SMTP (Simple Mail Transfer Protocol)       | Sends email between mail servers and from clients to mail servers.                                                            | Email spoofing, spam relay, and phishing attacks if the server is not properly configured.                        |
| **53**    | DNS (Domain Name System)                   | Translates domain names into IP addresses.                                                                                    | DNS spoofing, cache poisoning, and DNS amplification attacks.                                                     |
| **80**    | HTTP (Hypertext Transfer Protocol)         | Delivers web pages over the internet without encryption.                                                                      | Data interception, man-in-the-middle attacks, and web application vulnerabilities.                                |
| **110**   | POP3 (Post Office Protocol v3)             | Retrieves email from a mail server to a local device.                                                                         | Credentials may be exposed if encryption is not used; susceptible to eavesdropping.                               |
| **143**   | IMAP (Internet Message Access Protocol)    | Allows users to access and manage email stored on a mail server.                                                              | Unencrypted connections can expose email data and login credentials.                                              |
| **443**   | HTTPS (Hypertext Transfer Protocol Secure) | Provides encrypted communication for secure web browsing.                                                                     | Weak SSL/TLS configurations, expired certificates, and protocol vulnerabilities.                                  |
| **445**   | SMB (Server Message Block)                 | Enables file and printer sharing on Windows networks.                                                                         | Vulnerable to malware, ransomware (such as WannaCry), and unauthorized file access if not secured.                |
| **3389**  | RDP (Remote Desktop Protocol)              | Allows remote access and control of Windows computers.                                                                        | Brute-force attacks, credential theft, and unauthorized remote access if exposed to the internet.                 |


# Part F: Scan Analysis

### 1. Which services are currently running?

The Nmap scan detected the following services running on the local machine:

* **Port 80:** HTTP (Microsoft IIS Web Server)
* **Port 135:** Microsoft RPC (Remote Procedure Call)
* **Port 445:** Microsoft-DS (SMB – Server Message Block)

### 2. Are all open ports necessary?

Not necessarily. Some ports are required for the operating system or installed applications to function correctly. However, services that are not being used should be disabled to reduce the system's attack surface.

### 3. Which services could become security risks if misconfigured?

The **HTTP (Port 80)** service could expose web applications to attacks if it is not properly configured. **Microsoft RPC (Port 135)** and **SMB (Port 445)** can also become security risks if they are exposed to untrusted networks or left unpatched, as they have been targeted by malware and unauthorized access attempts.

### 4. Which port would you disable if it wasn't required?

If file and printer sharing is not needed, I would disable **Port 445 (SMB)** because it has been associated with several security vulnerabilities and malware attacks. Disabling unused services helps improve system security.






