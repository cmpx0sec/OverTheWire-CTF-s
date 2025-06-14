# Level 17: Bandit - OverTheWire

**🎯Objective:**  
There are two files in the home directory: passwords.old and passwords.new. The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new

---

## 📝 Steps Taken
Simple Level, minimal to no steps needed 

## 💡Solution:

To obtain the password for this level, we will need to use a new command, **diff**. This command helps look at the differences between two files,

  Command:
   ```bash
   diff passwords.old passwords.new
```
This will output the two lines, the top line is from the file 'passwords.old' and replaces the bottom line from 'passwords.new'

## 🔑 Password for Level 18:
x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO

## 🛠️ Tools and Commands Learned

**diff** - helps compare the contents of different files

## 🔍 Proof of Execution

![image](https://github.com/user-attachments/assets/f5ee8d1f-89dd-43ed-8dab-78ee8121c4c7)
