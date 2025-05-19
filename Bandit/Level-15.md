# Level 15: Bandit - OverTheWire

**🎯Objective:**  
The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL/TLS encryption.

---

## 📝 Steps Taken
 1. Logged into the bandit server as **bandit15**
 2. Connected to port **3001** on **localhost** using the **openssl** client to establish a secure connection

## 💡Solution:
To make a secure connection and send the password:

  Command:
   ```bash
   openssl s_client -connect localhost:30001
```
After the connection is established, paste the level 15 password: 8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
The password will be shown after entering the level 15 password.

## 🔑 Password for Level 16:
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx

## 🛠️ Tools and Commands Learned
**openssl s_client**: Connects to a remote host using SSL/TLS
Secure Communication via **localhost** and custom ports 

## 🔍 Proof of Execution
![image](https://github.com/user-attachments/assets/c4b06119-fc0d-48a0-9801-1fe596e9f459)
![image](https://github.com/user-attachments/assets/0323fdfe-95ec-40a4-9997-4c898d1940c0)

