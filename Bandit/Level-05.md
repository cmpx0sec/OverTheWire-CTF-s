# Level 05: Bandit - OverTheWire

**🎯Objective:**  
The goal of this level is to locate and retrieve the password within the *inhere* directory. the correct file has specific attributes (non-executable, 1033 bytes, Human-readable) 

---

## 📝 Steps Taken
1. Navigate to the *inhere* directory, thier are mutliple directories, it would take to long to look at them all one by one.
2. The password is stored in a file with specific criteria, using the *find* command will help filter files based on size and file type
3. Once the correct file is identified the contents within the file (the password) can be retrieved for the next level 


## 💡Solution:

The following command was used to locate and display the password:

  Command:
   ```bash
   find -size 1033c ! -executable
```
The password is inside this file.

## 🔑 Password for Level 00:
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

## 🛠️ Tools and Commands Learned


## 📝 Notes
1. Understanding file attributes is imperetive for system navigation
2. File inspection and filtering are essential for forensic analysis, privlege escalation and vulnerabillity assesments

## 🔍 Proof of Execution
![image](https://github.com/user-attachments/assets/5a349352-d828-4a5e-a638-4907543cbba1)
