# Level 12: Bandit - OverTheWire

**🎯Objective:**  
The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

---

## 📝 Steps Taken
1. created a temporary working directory in /tmp
2. Copied data.txt to the temporary directory
3. Reversed the hexdump to binary format
4. Decompressed multiple layers of compression (gzip, bzip2, tar archives)
5. Repeated decompression until reaching the final ASCII text file

## 💡Solution:
First reversed the hexdump:

  Command:
   ```bash
   xxd -r data.txt > data
```

then went through decompression cycles:

 Command:
   ```bash
   # First layer (gzip)
mv data data.gz
gzip -d data.gz

# Second layer (bzip2)
bzip2 -d data

# Third layer (gzip again)
mv data.out data.gz
gzip -d data.gz

# Fourth layer (tar archive)
tar -xf data

# Fifth layer (bzip2 again)
bzip2 -d data5.bin

# Sixth layer (tar archive again)
tar -xf data5.bin.out

# Final layer (gzip)
mv data6.bin data6.gz
gzip -d data6.gz
```

The password is inside the final decompressed file.

## 🔑 Password for Level 13:
FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn

## 🛠️ Tools and Commands Learned
**xxd -r** - Reverse hexdump to binary

**gzip -d** - Decompress gzip files

**bzip2 -d** - Decompress bzip2 files

**tar -xf** - Extract tar archives

**file** - Determine file type

**mktemp -d** - Create secure temporary directory

**File compression formats** - Understanding of nested compression techniques

## 🔍 Proof of Execution
![image](https://github.com/user-attachments/assets/d6cd924d-f0c7-432b-9e2a-de51c6657a7a)

![image](https://github.com/user-attachments/assets/f1f8556c-89b1-4ad4-9076-5a64ccc4b3de)

