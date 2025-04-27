# Level 02: Bandit - OverTheWire

**Objective:**  
The goal for **Level 2** is to open files that have spaces

---

## 📝 Steps Taken
The file in the home directory has spaces in its name which means it must be handled diffrentley when using the **cat** command.

## Solution:
When a filename contains spaces, wrap the filename in quotation marks ("")

  Command:
   ```bash
   cat "spaces in the filename"
```
Password is inside this file.

## 🔑 Password for Level 3:
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

## 🛠️ Tools and Commands Learned
"": wrapping filenames in quotation marks when filename has spaces

## 📝 Notes
To correctly reference a file when said file has spaces in its name, one must wrap it in quotation marks or use an escape character in bettween the spaces of the file name in order to access it's contents.
