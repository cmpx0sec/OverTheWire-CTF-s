# Level 20: Bandit - OverTheWire

**🎯Objective:**  

There is a setuid binary in the home directory that does the following: it makes a connection to localhost on the port specified as a command-line argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

---

## 📝 Steps Taken
Look in the home directory, and there will be a binary named **suconnect**. Using netstat will help see what ports are listening on the system.

The next step is to set up a netcat listener on port 1234 in the background and piping the current level's password to this listener with the following command;

  Command:
   ```bash
   echo "0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO" | nc -nlvp 1234 &
```

## 💡Solution:
Next, run the following command;

  Command:
   ```bash
   ./suconnect 1234
```
The password will be shown after the connection is established. 

## 🔑 Password for Level 21:
EeoULMCra2q0dSkYj561DX7s1CpBuOBt

## 🛠️ Tools and Commands Learned

**netstat** - a command-line tool used to display network connections, routing tables, and interface statistics

## 🔍 Proof of Execution

![image](https://github.com/user-attachments/assets/296862ad-3942-4f29-8878-720365209d9c)
