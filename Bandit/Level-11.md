# Level 11: Bandit - OverTheWire

**🎯Objective:**  
The password for the next level is stored in the file **data.txt**, where all lowercase and uppercase letters have been rotated by 13 positions

---

## 📝 Steps Taken
1. Navigate to the **data.txt** file and open file
2. There is a string of data, the objective states that this string has been rotated by 13 positions, which is a Caesar cipher ROT13 https://en.wikipedia.org/wiki/ROT13, This means the alphabet letters have been rotated 13 times to make a new string that makes no sense at first glance
3. Just as in the previous level, some websites can be used, such as https://cryptii.com/pipes/caesar-cipher will help solve this level easily, however, there is also another way to solve this using the terminal  

## 💡Solution:
This command will help rotate the password back to the original alphabet 

  Command:
   ```bash
   echo Gur cnffjbeq vf 7k16JArUVv5LxVuJfsSVdbbtaHGlw9D4 | tr A-Za-z  N-ZA-Mn-za-m
```
The output will be the string decoded in the origional alphabet (as seen in the image below)

## 🔑 Password for Level 12:
7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4

## 🛠️ Tools and Commands Learned
**tr** - (short for translate) used to replace, delete, or squeeze characters in text input.

## 🔍 Proof of Execution
![image](https://github.com/user-attachments/assets/13635418-145a-4a95-8909-1045a33dc87e)
