# Level 00: Krypton - OverTheWire

**🎯 Objective**

The following string encodes the password using Base64:  
`S1JZUFRPTklTR1JFQVQ=`

Use this password to log in to `krypton.labs.overthewire.org` with username `krypton1` using SSH on port `2231`.

---

## 💡 Solution

### 1) Decode the Base64 string to get the password for `krypton1`

Run one of these locally:

```bash
# Using the base64 utility
echo 'S1JZUFRPTklTR1JFQVQ=' | base64 --decode

# OR using Python if base64 isn't available
python3 -c "import base64; print(base64.b64decode('S1JZUFRPTklTR1JFQVQ=').decode())"
```
<img width="662" height="160" alt="image" src="https://github.com/user-attachments/assets/dd2303f4-9edc-4278-9c67-e097dadb662d" />

### 2) SSH into Krypton host
```bash
ssh krypton1@krypton.labs.overthewire.org -p 2231
# when prompted, paste the password from the previous step
```

### 3) Find the file with the password for level 1
after going into directories thier is a `README` file that has an introductory message about where the password for the next level is and how it is encrypted (also says not to use cryptool....)

<img width="894" height="860" alt="image" src="https://github.com/user-attachments/assets/3abfca5f-3180-4e30-aa50-e282a3239b4e" />

### 4) Go to `krypton2` file and decode it 
It is mentioned in the `README` file that this is a simple Ceaser Cipher, ROT13 (Rotate the alphabet 13 times)
Thier are external resourses that can help with decrypting but this will be done on the terminal with the following command:
```bash
echo 'YRIRY GJB CNFFJBEQ EBGGRA' | tr 'A-Za-z' 'N-ZA-Mn-za-m'
# The output should be the awnser 
```
<img width="894" height="230" alt="image" src="https://github.com/user-attachments/assets/da85dc11-e8df-4d69-9a0f-32fe9dcb19a6" />
