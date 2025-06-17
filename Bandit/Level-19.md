# Level 19: Bandit - OverTheWire

**🎯Objective:**  
To gain access to the next level, use the setuid binary in the home directory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after the setuid binary has been used.

---

## 📝 Steps Taken
Check the home directory, there will be a binary named bandit20-do. Next, check permissions by typing the command;

Command:
   ```bash
   file bandit20-do
```
There will be an output of information that looks something like "setuid ELF 32-bit LSB executable" 


## 💡Solution:

To read the password file (/etc/bandit_pass/bandit20), execute:

  Command:
   ```bash
   ./bandit20-do cat /etc/bandit_pass/bandit20
```
The password should be outputed after this command.

## 🔑 Password for Level 20:
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO

## 🛠️ Tools and Commands Learned

**setuid** 

## 🔍 Proof of Execution

![image](https://github.com/user-attachments/assets/b15951dc-6437-46c7-a797-5c542562131f)
