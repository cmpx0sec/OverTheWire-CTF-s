# Level 06: Bandit - OverTheWire

**🎯Objective:**  
The goal of this level is to find the password somewhere within the server. the file that has the password is owned by user bandit7, owned by group bandit6 and 33 bytes in size

---

## 📝 Steps Taken
1. Navigate to the **home** directory, this directory contains numerous subdirectories, making manual inspection inefficent
2. The password is stored in a file with specific criteria, using the *find* command will help filter files based on size and file type
3. Once the correct file is identified the contents within the file (the password) can be retrieved for the next level 

## 💡Solution:
The following command was used to locate where the password is hidden:

  Command:
   ```bash
   find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
```
This command helps search the entire server, helps go through all the files that are owned by user bandit7 and group bandit6 and it will help find files that are specifically 33 bytes in size. Note the last part of the command (2>/dev/null) helps hide any error messages that may occur 

Once the command has been inputed the output will be the file path of where the password is the file path should be, /var/lib/dpkg/info/bandit7.password, navigate to the file using the following command;

 Command:
   ```bash
   cat /var/lib/dpkg/info/bandit7.password
```
The password will appear after inputing the above command

## 🔑 Password for Level 07:
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

## 🛠️ Tools and Commands Learned
1. **/** - this symbol helps search the entire file system
2. **-type f** - this portion of the command helps only search files in the server (excludes directories)
3. **2>/dev/null** - helps hide error messages

## 📝 Notes
1. file ownership is important - ownership is important for privilege escalation and forensics
2. error suppression - **2>/dev/null** is a standard tool for filtering noise in system searches (used in penetration testing).
3. Real-World Applications - for forensic investigations, asking who owns a file is a common question when tracing breaches 
   

## 🔍 Proof of Execution
![image](https://github.com/user-attachments/assets/eb60b39f-6446-46a6-945c-2692bcd3495b)
