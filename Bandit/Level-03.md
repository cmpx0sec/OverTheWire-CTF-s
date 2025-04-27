# Level 03: Bandit - OverTheWire

## **🎯Objective:**  
Find file that is hidden somewhere in the directory 

---

## 📝 Steps Taken
When in the home directory thier is no file, only a directory called **inhere**
To move directory and find the file you must input the following command;

Command:
   ```bash
   cd
```
The file in the **inhere** directory is hidden that means the **ls** command on its own will result in no files appearing 

## Solution:
When a filename is hidden write the command below. This command lists the contents of a directory in a detailed human-readable format. 

  Command:
   ```bash
   ls -la
```

- **-l** lists all the detailed information
- **-a** lists all hidden files

you should see something like this come up once the command above is written;
![image](https://github.com/user-attachments/assets/e4317e1b-6f09-4fc1-9bec-f5a881fb85e0)

you could also just write;

   ```bash
   ls -a
```
This command will give the hidden file without the extra information and it will look like this;
![image](https://github.com/user-attachments/assets/56577c91-53e7-46a8-95bb-6e22e84cf4d7)

the filename is now presented to the user and using the lesson from [Level 2]





Password is inside this file.

## 🔑 Password for Level 3:

## 🛠️ Tools and Commands Learned

## 📝 Notes
