# Level 16: Bandit - OverTheWire

**🎯Objective:**  
The credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. First, find out which of these ports have a server listening on them. Then, find out which of those speak SSL/TLS and which don’t. Only one server will provide the next credentials; the others will return whatever is sent to them.

---

## 📝 Steps Taken

Port scanning:

Command:
   ```bash 
   nmap -vv -p31000-32000 -sV -T5 localhost
```
The command above will help scan all ports from 31000 to 32000, state what is open, and identify the service behind each port. Next, after the scan finishes, there will be an output of different ports, one of which will accept input and return the RSA private key. To do this, run the following command;

Command:
   ```bash
   echo 'kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx' | openssl s_client -quiet -connect localhost:31790
```
For this level, this specific command helps find the RSA private key, as shown in the image below. Now that the RSA private key has been found 

## 💡Solution:


  Command:
   ```bash
   
```
The password is inside this file.

## 🔑 Password for Level 17:
RSA Private key

## 🛠️ Tools and Commands Learned

**nmap** – to scan for open ports

**nc (netcat)** – to send data to open ports and receive responses

**echo** – to automate input to the service

**ssh** – to connect using the retrieved RSA key

**chmod** – to secure the private key file

## 🔍 Proof of Execution
![image](https://github.com/user-attachments/assets/16bb923e-b220-4a01-839f-a3d674d7b067)

![image](https://github.com/user-attachments/assets/6a485dfc-a0ef-4878-9605-9cbe9b3b7b7f)
