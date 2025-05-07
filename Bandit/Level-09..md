# Level 09: Bandit - OverTheWire

**🎯Objective:**  
Find the password in the **data.txt** file that is base64 encoded
 
---

## 📝 Steps Taken
1. Navigate to the file and open it. There is a string of data that is base64 encoded
2. To solve this level and get the password, the string must be decoded
3. When the string is found, there are two ways to solve this level: either by going online and decoding it with a website such as https://www.base64decode.org/ or using the linux terminal

## 💡Solution:

  Command:
   ```bash
   echo VGhlIHBhc3N3b3JkIGlzIGR0UjE3M2ZaS2IwUlJzREZTR3NnMlJXbnBOVmozcVJyCg== | base64 --decode 
```

This will output the decoded version which is "The password is dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr" 
The echo command printed the Base64-encoded string:

VGhlIHBhc3N3b3JkIGlzIGR0UjE3M2ZaS2IwUlJzREZTR3NnMlJXbnBOVmozcVJyCg==

Then the pipe command sent the output to the next command (base64). Finally, base64 --decode decoded the string to reveal the original message.

## 🔑 Password for Level 10:
dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

## 🛠️ Tools and Commands Learned
**echo** - Prints text/variables to the terminal or redirects to files.
**base64 --decode** - Decodes Base64-encoded data into its original form.

## 🔍 Proof of Execution
![image](https://github.com/user-attachments/assets/7e2e0770-0292-4ad0-8a50-d9fe889c1269)
