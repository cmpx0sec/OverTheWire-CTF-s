# Level 09: Bandit - OverTheWire

**🎯Objective:**  
to find the human-readable strings preceded by several equal characters

---

## 📝 Steps Taken
1. In the overthewire page for this level, **strings** are mentioned 
2. The following command was the command initially used to look at any human-readable data;


   Command:
   ```bash
   strings data.txt
```

3. This command gives all strings within the file, where there are equal characters next to human-readable words such as "the", "password", "is", and equal characters next to a line that looks like the password


## 💡Solution:
because there are lots of strings to shorten the data that is outputted, the **grep** command will be used 

  Command:
   ```bash
   strings data.txt | grep =
```
The output only shows and highlights strings with equal characters. The password is now obvious.
Note: I also tested multiple equal characters (as seen below in the proof of execution section) by adding more equal characters, the number of strings will shorten and even look like a sentence going from the top down

## 🔑 Password for Level 10:
FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey

## 🛠️ Tools and Commands Learned
**strings** - A  sequence of characters (letters, numbers, symbols, or spaces) treated as textual data rather than binary code.

**grep** - Helps search text patterns in files or input streams

## 🔍 Proof of Execution
![image](https://github.com/user-attachments/assets/24331134-76b6-4fe4-af54-05ce67fff163)

I also wanted to see what would happen if I put multiple equal symbols, the list shortened, and it appears to say "the password is FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey"

![image](https://github.com/user-attachments/assets/790e743c-0804-4599-8b1e-2ee0e736ec1c)
