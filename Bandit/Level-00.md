# Level 00: Bandit - OverTheWire

**Objective:**  
The goal for **Level 0** is to log in to the Bandit server using SSH with the username "bandit0" and find the password for **Level 1**.

---

## 📝 Steps Taken

1. **Access the Bandit server**:
   The first step is to log in using SSH. The credentials are given in the welcome message when you start the game.

   Command:
   ```bash
   ssh bandit0@bandit.labs.overthewire.org -p 2220
   
You’ll be prompted for the password, which will be **bandit0** as stated in the instructions on https://overthewire.org/wargames/bandit/bandit0.html .

---

2. **Navigating The Terminal**

To find the file containing the password for the next level, use the ls command to list the files in the current directory.

   Command:
   ```bash
   cat

---
You should see a file called **readme**. This is the file you need to open to get the password for Level 1.

Read the readme file:
Now, use the cat command to display the contents of the file and find the password.

Command:
   ```bash
   ls

---
Once the file is opened you should see the password

##🔑 Password for Level 1:
boJ9jbbUNNfktd78OOpsqOlt2aP7a3v7

##🛠️ Tools and Commands Learned
SSH: Used to log in to remote servers.

ls: List the contents of the current directory.

cat: Display the contents of a file.

##📝 Notes
- The welcome message is important! It often contains the clue for finding the password.
- The password is stored in the readme file in the home directory.
- Be sure to use cat to view file contents in this type of challenge.

Next Steps:
With the password from Level 0, log in to Level 1 and repeat the process for the next challenge.

---
