# Level 18: Bandit - OverTheWire

**🎯Objective:**  
The password for the next level is stored in a file, readme, in the home directory. Unfortunately, someone has modified .bashrc to log the user out when they log in with SSH.

---

## 📝 Steps Taken
Simple Level, minimal to no steps needed

## 💡Solution:

  Command:
   ```bash
   ssh -i id_rsa bandit18@bandit.labs.overthewire.org -p 2220 "cat readme"
```
Input the password from the previous level, and the output will be the password for the next level 

## 🔑 Password for Level 19:
cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8

## 🛠️ Tools and Commands Learned

**ssh** - cryptographic network protocol for operating network services securely over an unsecured network

## 🔍 Proof of Execution

![image](https://github.com/user-attachments/assets/b795c381-dc11-4474-a79a-c56b27252a70)

