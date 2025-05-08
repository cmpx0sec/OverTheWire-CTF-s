# Level 14: Bandit - OverTheWire

**🎯Objective:**  
The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost.

---

## 📝 Steps Taken
1. Logged in as bandit14 using the password from level 13 → 14
2. Verified current level password in /etc/bandit_pass/bandit14
3. Submitted the password to localhost port 30000 using netcat

## 💡Solution:
The solution requires sending the current level's password to a network service on port 30000.

  Command:
   ```bash
   echo "4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e" | nc localhost 30000
```

## 🔑 Password for Level 15:
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo

## 🛠️ Tools and Commands Learned
**nc** (netcat) for network communication

**Piping** output to network services

Basic service interaction patterns

## 🔍 Proof of Execution
![image](https://github.com/user-attachments/assets/96ee7c9c-f7ef-482a-a025-3e6100fd31f2)
