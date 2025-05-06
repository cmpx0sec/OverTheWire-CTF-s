# Level 07: Bandit - OverTheWire

**🎯Objective:**  
The goal of this level is to find the word **millionth** next to this word, which is the password

---

## 📝 Steps Taken
1. For this level, look at what files there are, there should only be one with the name **data.txt**
2. If you open this file there will be a lot of text written out
3. For this level, the word **millionth** has to be found to find the password for the next level intrinsically. To do this, the grep command should be used
   
## 💡Solution:
The following command was used to locate the word that the password is next to:

  Command:
   ```bash
   grep millionth data.txt
```
This command helps find a specific word using **grep**. The command is followed by the word that needs to be located and the file in which it is located

The word **millionth** will be beside the password

## 🔑 Password for Level 08:
dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

## 🛠️ Tools and Commands Learned
1. **grep** - used for searching text or patterns in files

## 📝 Notes
1. Forensic application - grep is vital for analysing logs, memory dumps, or disk images during incident response.

## 🔍 Proof of Execution
![image](https://github.com/user-attachments/assets/13c9c787-7823-4f21-8030-baf1da161100)
