# Level 21: Bandit - OverTheWire

**🎯Objective:**  

A program runs automatically at regular intervals via cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

---

## 📝 Steps Taken
First, enumerate the cron.d directory with the following command:
```bash
   ls -la /etc/cron.d/
```
Thier is a cronjob for the next level:
```bash
   cat /etc/cron.d/cronjob_bandit22
```
Thier will be a script inside, run it
```bash
   cat /usr/bin/cronjob_bandit22.sh
```

## 💡Solution:
The script creates a file in the /tmp directory and copies the password for the next level:

   ```bash
   cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv

```

## 🔑 Password for Level 22:
tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q

## 🛠️ Tools and Commands Learned
cron > time based job scheduler

## 🔍 Proof of Execution
<img width="764" height="311" alt="image" src="https://github.com/user-attachments/assets/86869f16-4cae-4b95-a9d0-99f46211ad23" />

