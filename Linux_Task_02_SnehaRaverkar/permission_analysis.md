 # Part C: File Ownership

Original Owner:
sneha

New Owner:
student3

Command Used:
sudo chown student3 report.txt

Observation:
The ownership of report.txt was successfully changed from student1 to student3. This was verified using the ls -l command.

# Part D: File Permissions
File Name: security_policy.txt

1. Read Only (r--r--r--)
Command Used:
chmod 444 security_policy.txt
Observation:
All users can read the file, but nobody can modify or execute it.

2. Read & Write (rw-rw-r--)
Command Used:
chmod 664 security_policy.txt
Observation:
The owner and group can read and modify the file. Other users can only read it.

3. Full Access (rwxrwxrwx)
Command Used:
chmod 777 security_policy.txt
Observation:
All users can read, write, and execute the file. This permission is generally not recommended for sensitive files because it allows unrestricted access.




# Part E: Permission Analysis
## Permission Analysis

### Permission 755
Owner Rights: Read, Write, Execute
Group Rights: Read, Execute
Other User Rights: Read, Execute

Use Case:
Used for directories and executable files where the owner can modify the file and others can access it.

### Permission 644
Owner Rights: Read, Write
Group Rights: Read
Other User Rights: Read

Use Case:
Used for documents and configuration files that only the owner should edit.

### Permission 777
Owner Rights: Read, Write, Execute
Group Rights: Read, Write, Execute
Other User Rights: Read, Write, Execute

Use Case:
Provides full access to everyone. Generally avoided due to security risks.

### Permission 600
Owner Rights: Read, Write
Group Rights: No Access
Other User Rights: No Access

Use Case:
Used for sensitive files such as passwords and private keys.

### Permission 700
Owner Rights: Read, Write, Execute
Group Rights: No Access
Other User Rights: No Access

Use Case:
Used for private directories and personal scripts.
