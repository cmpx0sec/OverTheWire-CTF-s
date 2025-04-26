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
You’ll be prompted for the password, which you’ll find in the welcome message after logging in.

Welcome Message:
Once you successfully log in, you’ll be greeted with a welcome message. This message often contains a clue or the password you need for the next level.

Example output:

pgsql
Copy
Edit
Bandit lvl 0 -> lvl 1

The password for the next level is stored in a file called "readme" in the home directory.
This message tells you that the password for Level 1 is in a file called readme in the home directory.

List the contents of the home directory:
To find the file containing the password for the next level, use the ls command to list the files in the current directory.

Command:

bash
Copy
Edit
ls
You should see a file called readme. This is the file you need to open to get the password for Level 1.

Read the readme file:
Now, use the cat command to display the contents of the file and find the password.

Command:

bash
Copy
Edit
cat readme
The contents of the file will give you the password for Level 1.

🔑 Password for Level 1:
boJ9jbbUNNfktd78OOpsqOlt2aP7a3v7

🛠️ Tools and Commands Learned
SSH: Used to log in to remote servers.

ls: List the contents of the current directory.

cat: Display the contents of a file.

📝 Notes
The welcome message is important! It often contains the clue for finding the password.

The password is stored in the readme file in the home directory.

Be sure to use cat to view file contents in this type of challenge.

Next Steps:
With the password from Level 0, log in to Level 1 and repeat the process for the next challenge.

yaml
Copy
Edit

---

This should now be formatted properly for GitHub Markdown. You can copy and paste this dire
