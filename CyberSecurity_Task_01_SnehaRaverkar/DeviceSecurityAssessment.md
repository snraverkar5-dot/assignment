# Security Assessment of Personal Computer/Laptop

## System Security

### 1. Operating System

**Method Used:**

* Press `Windows + R`
* Type `winver`
* Press Enter

**Command Used:**

```text
winver
```

**Result:**
The operating system installed on my laptop is Windows 11.

---

### 2. OS Version

**Method Used:**

* Open the Run dialog using `Windows + R`
* Type `winver`
* Press Enter
* The Windows version information is displayed

**Command Used:**

```text
winver
```

**Result:**
The OS version of my system is displayed in the Windows About window.

---

### 3. Is the System Updated?

**Method Used:**

* Open **Settings**
* Go to **Windows Update**
* Check the update status

**Result:**
Yes, my system is updated with the latest Windows updates and security patches.

---

### 4. Antivirus Installed?

**Method Used:**

* Open **Windows Security**
* Select **Virus & Threat Protection**
* Check whether antivirus protection is active

**Command Used (PowerShell):**

```powershell
Get-MpComputerStatus
```

**Result:**
Yes, Microsoft Defender Antivirus is installed and active on my system.

---

### 5. Firewall Enabled?

**Method Used:**

* Open **Windows Security**
* Select **Firewall & Network Protection**
* Verify that the firewall is turned on

**Command Used (Command Prompt):**

```cmd
netsh advfirewall show allprofiles
```

**Result:**
Yes, Windows Firewall is enabled and protecting the system.

---

## Conclusion

I checked the security settings of my laptop using Windows tools and commands. The operating system is Windows 11, the system is updated, Microsoft Defender Antivirus is active, and Windows Firewall is enabled. These security features help protect the computer from malware, unauthorized access, and other cyber threats.

## Screenshots Attached

1. Output of `winver` (Operating System and OS Version)
2.. Virus & Threat Protection Page
3. Firewall & Network Protection Page

