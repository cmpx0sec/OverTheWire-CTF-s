# Level 08: Bandit - OverTheWire

**🎯Objective:**  
to find the line of data that only occurs once, that is the password for the next level

---

## 📝 Steps Taken
1. When navigating to the file named **data.txt** and opening it, a lot of data is repeated. For this level, there is a unique line hidden within the data that is the password
2. The **sort** command is used to sort through files numerically/alphabetically
3. The **uniq** command helps get rid of any repetition in the chosen file
4. These commands will be helpful in this level's context. They will both help identify the unique line (the password)

## 💡Solution:
The following command is used to help find the password to the next level;

  Command:
   ```bash
   sort data.txt | uniq -u
```
This command uses **piping**, which helps chain different commands together. Notice that **uniq** has **-u** adjacent to it, because **-u** only outputs lines that are unique in the input. When using **uniq -u**, it will output the password alone.

## 🔑 Password for Level 09:
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM

## 🛠️ Tools and Commands Learned
**sort** - Orders lines alphabetically (groups duplicates).
**uniq -u** - Only output lines that are unique in the input.
**piping** - chains commands together, passing the output of one command as input to the next. 

## 📝 Notes
These commands can be utilised in situations related to hidden passwords, such as steganography in log files or attackers masking malicious activity in normal traffic

## 🔍 Proof of Execution
![image](https://github.com/user-attachments/assets/eaf91ce6-2738-48e2-8cc7-d345b8a8f1d1)


