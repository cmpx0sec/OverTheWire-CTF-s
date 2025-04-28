
# Level 04: Bandit - OverTheWire

**🎯Objective:**  
To discover which file is human readable

---

## 📝 Steps Taken

Go into the **inhere** directory and look inside the directory, Thier are 10 different files 

![image](https://github.com/user-attachments/assets/1e3dbf4b-814c-440b-a0d0-e38a69ee3908)


## 💡Solution:

instead of going through each file one by one, look through the all the files at once using the command;

Command:
   ```bash
   file ./*
```
The files should all appear with the type of information that is inside each file

![image](https://github.com/user-attachments/assets/7a579154-c847-4ed1-a8ef-05361f34565c)

for this instance **-file07** is the odd one out so check the file content by opening the file 

![image](https://github.com/user-attachments/assets/1a470bd0-fac2-444a-8b86-41beb4772416)

The password is inside this file.

## 🔑 Password for Level 5:
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

## 🛠️ Tools and Commands Learned
file - determines file type 
