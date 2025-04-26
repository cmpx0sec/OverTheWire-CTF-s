# Level 01: Bandit - OverTheWire

**Objective:**  
The goal for **Level 1** is to open files that start with special characters

---

## 📝 Steps Taken
1. **Access the Bandit server**:
Using the password we found from the previous level we access **bandit1**.

2. **Looking into Directory**:
The first thing we do is list all the files in the current directory the same way we did originally

  Command:
   ```bash
   ls
```
3. **Special Characters**:
Normally we would just write the **cat** command along with the name of the file but this time the file name is simply a dash symbol **-**.
Normally opening the file with the **cat** command alone will result in the terminal not responding when dealing with a file starting with a special character instead you must use the following command;

Command:
   ```bash
   cat ./-
```
the **./** command 


##🔑 Password for Level 2:
263JGJPfgU6LtdEvgfWU1XP5yac29mFx

##🛠️ Tools and Commands Learned
./: 

##📝 Notes

---

   
   
