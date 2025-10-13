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

 

<img width="662" height="160" alt="image" src="https://github.com/user-attachments/assets/dd2303f4-9edc-4278-9c67-e097dadb662d" />

