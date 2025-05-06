# Level 05: Bandit - OverTheWire

**🎯Objective:**  
The goal of this level is to locate and retrieve the password within the *inhere* directory. The correct file has specific attributes (non-executable, 1033 bytes, Human-readable) 

---

## 📝 Steps Taken
1. Navigate to the **inhere** directory, this directory contains numerous subdirectories, making manual inspection inefficient
2. The password is stored in a file with specific criteria. Using the *find* command will help filter files based on size and file type
3. Once the correct file is identified, the contents within the file (the password) can be retrieved for the next level 

## 💡Solution:
The following command was used to locate the password:

  Command:
   ```bash
   find -size 1033c ! -executable
```
The output of this command will give both the directory and the file where the password is hidden (./maybehere07/.file2), navigate to that directory and then navigate to the file, the password will be inside.

## 🔑 Password for Level 06:
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

## 🛠️ Tools and Commands Learned
1. **find** - used for file and directory searches, search files by attributes 
2. **! -executable** - the exclamation mark in this part of the command means **NOT** executable
3. **-size 1033c** - matches files by byte size 

## 📝 Notes
1. Understanding file attributes is imperative for system navigation
2. Real-World Applications:
   
   Forensics: Identifying suspicious files by metadata.
   
   Privilege Escalation: Hunting for misconfigured permissions.
   
   Vulnerability Assessments: Scanning for exposed sensitive data.

## 🔍 Proof of Execution
![image](https://github.com/user-attachments/assets/5a349352-d828-4a5e-a638-4907543cbba1)
