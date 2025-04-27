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
Normally, we would use the cat command followed by the file name. However, this time the file name is a single dash symbol (-).
Running cat - would not open the file correctly — it would cause the terminal to hang because - is interpreted as an option, not a file name.
Instead, we must specify the file path explicitly using ./, which tells the terminal to look for a file named - in the current directory.

Command:
   ```bash
   cat ./-
```
the **./** command 


## 🔑 Password for Level 2:
263JGJPfgU6LtdEvgfWU1XP5yac29mFx

## 🛠️ Tools and Commands Learned
./: Refers to the current directory. This command is useful when accessing files with special/confusing names.

## 📝 Notes
Files that start with special characters (like -) should be accessed using ./ to avoid misinterpretation by the command line.

---

   
   
