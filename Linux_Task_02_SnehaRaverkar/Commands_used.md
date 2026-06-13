# PartA understanding Users
1. whoami
   - Shows the current username.

2. id
   - Shows the User ID (UID), Group ID (GID), and group information.

3. cat /etc/passwd
   - Displays information about all user accounts stored on the Linux system.



# Part B 
## To create users and group

  ### Create groups
sudo groupadd interns
sudo groupadd cyberteam

### Create users
sudo useradd student1
sudo useradd student2
sudo useradd student3

### Add users to groups
sudo usermod -aG interns student1
sudo usermod -aG cyberteam student2
sudo usermod -aG interns student3

### Verify group membership
groups student1
groups student2
groups student3

### Display user and group IDs
id student1
id student2



# Part C: File Ownership
## File Ownership Commands

### Create Project Folder
mkdir CyberSecurity_Project

### Move into Folder
cd CyberSecurity_Project

### Create Files
touch report.txt
touch notes.txt
touch credentials.txt

### Check File Ownership
ls -l

### Change Ownership
sudo chown student3 report.txt

### Verify Ownership Change
ls -l



# Part D: File Permissions
## File Permission Commands

### Create File
touch security_policy.txt

### Check Current Permissions
ls -l security_policy.txt

### Set Read Only Permissions
chmod 444 security_policy.txt
ls -l security_policy.txt

### Set Read and Write Permissions
chmod 664 security_policy.txt
ls -l security_policy.txt

### Set Full Access Permissions
chmod 777 security_policy.txt
ls -l security_policy.txt
  
