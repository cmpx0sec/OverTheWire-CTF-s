# Level 22: Bandit - OverTheWire

**🎯Objective:**  

A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

---

## 📝 Steps Taken
Look at the cronjob (similar to the previous level)
```bash
   cat /etc/cron.d/cronjob_bandit23
```
And then the script:
```bash
   cat /usr/bin/cronjob_bandit23.sh
```
It reveals a cronjob that is set to run every minute. Thier will be a script that cron runs (as shown below)
Replicate the script so it figures out the filename in /tmp/
  ```bash
   echo 'I am user bandit23' | md5sum
```
The result > 8ca319486bfbbc3663ea0fbe81326349
open the file that the cronjob script creates.

## 💡Solution:

This file contains the password.
   ```bash
   cat /tmp/8ca319486bfbbc3663ea0fbe81326349
```

## 🔑 Password for Level 23:
0Zf11ioIjMVN551jX3CmStKLYqjk54Ga

## 🛠️ Tools and Commands Learned
md5sum > used to verify the integrity of files by generating and checking MD5 checksums

## 🔍 Proof of Execution
<img width="792" height="481" alt="image" src="https://github.com/user-attachments/assets/5f5e5922-12e2-4497-8cc9-a8190c08ae3b" />


