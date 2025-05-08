# Level 13: Bandit - OverTheWire

**🎯Objective:**  
The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. A password is not required for this level, but a private SSH key can be used to log into the next level.

---

## 📝 Steps Taken
1. Connected to the server using the provided private SSH key
2. Logged in as bandit14 using the key authentication
3. Read the password for level 14 from the protected file


## 💡Solution:
This level requires using SSH key authentication instead of a password. The private key is stored in the home directory as sshkey.private.

  Command:
   ```bash
   ssh -i sshkey.private -p 2220 bandit14@localhost
```

After logging in, retrieve the password with:

Command:
   ```bash
   cat /etc/bandit_pass/bandit14
```

## 🔑 Password for Level 14:
[The actual password from /etc/bandit_pass/bandit14] 

## 🛠️ Tools and Commands Learned
SSH key authentication (-i flag)

Private key file permissions (chmod 600)

Reading protected system files

## 🔍 Proof of Execution

![image](https://github.com/user-attachments/assets/98861e20-f3e0-480e-a853-a974a3a05432)

![image](https://github.com/user-attachments/assets/f230d4b7-cb70-47ed-ae94-2b9083f33bbc)

