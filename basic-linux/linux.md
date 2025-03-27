# LINUX
# Basic Linux Command Reference (Ubuntu 20.04)

This document summarizes essential Linux commands, their syntax, and usage examples.  
Use it as a quick reference for day-to-day terminal tasks.

---

## 1. `pwd`
**What it does**  
Prints the current working directory path.

**Syntax**  
```bash
pwd
```
Example
```bash
pwd
# e.g. Output: /home/username
```

---
## 2. `ls`

### What it does
Lists files and directories in the current directory.

### Syntax
```bash
ls [OPTIONS] [FILE...]
```
Examples
```bash
ls
# Lists contents of the current directory

ls -l
# Lists contents in a detailed (long) format

ls -a
# Lists all files, including hidden ones

```



---

## 3. `cd`
**What it does**  
Changes the current working directory.

**Syntax**  
```bash
cd DIRECTORY
```

**Examples**  
```bash
cd /home/username/Documents
# Moves into the 'Documents' directory

cd ..
# Moves one directory up

cd ~
# Moves to the home directory of the current user
```

---

## 4. `mkdir`
**What it does**  
Creates a new directory.

**Syntax**  
```bash
mkdir DIRECTORY_NAME
```

**Example**  
```bash
mkdir new_folder
# Creates a directory named 'new_folder'
```

---

## 5. `rmdir`
**What it does**  
Removes an empty directory.

**Syntax**  
```bash
rmdir DIRECTORY_NAME
```

**Example**  
```bash
rmdir new_folder
# Removes 'new_folder' if it is empty
```

---

## 6. `cp`
**What it does**  
Copies files or directories.

**Syntax**  
```bash
cp [OPTIONS] SOURCE DESTINATION
```

**Examples**  
```bash
cp file1.txt file2.txt
# Copies file1.txt to file2.txt

cp -r folder1 folder2
# Recursively copies 'folder1' to 'folder2'
```

---

## 7. `mv`
**What it does**  
Moves or renames files and directories.

**Syntax**  
```bash
mv [OPTIONS] SOURCE DESTINATION
```

**Examples**  
```bash
mv oldfile.txt newfile.txt
# Renames 'oldfile.txt' to 'newfile.txt'

mv file.txt /home/username/Documents/
# Moves 'file.txt' into the Documents directory
```

---

## 8. `rm`
**What it does**  
Removes files or directories.

**Syntax**  
```bash
rm [OPTIONS] FILE...
```

**Examples**  
```bash
rm file.txt
# Removes 'file.txt'

rm -r folder
# Removes 'folder' and all its contents
```
> **Caution**: This is permanent deletion—use carefully.

---

## 9. `touch`
**What it does**  
Creates an empty file or updates the last modified timestamp of an existing file.

**Syntax**  
```bash
touch FILENAME
```

**Example**  
```bash
touch newfile.txt
# Creates 'newfile.txt' if it doesn't already exist
```

---

## 10. `cat`
**What it does**  
Displays the contents of a file.

**Syntax**  
```bash
cat FILENAME
```

**Example**  
```bash
cat file.txt
# Outputs the contents of file.txt to the terminal
```

---

## 11. `less`
**What it does**  
Displays file contents in a scrollable viewer.

**Syntax**  
```bash
less FILENAME
```

**Example**  
```bash
less file.txt
# Opens file.txt in a scrollable viewer
```
> Press `q` to quit.

---

## 12. `grep`
**What it does**  
Searches for lines matching a given pattern (string or regex).

**Syntax**  
```bash
grep [OPTIONS] PATTERN [FILE...]
```

**Examples**  
```bash
grep "hello" file.txt
# Displays lines in file.txt containing 'hello'

ls -l | grep ".txt"
# Searches for lines containing ".txt" in the output of ls -l
```

---

## 13. `find`
**What it does**  
Searches for files in a directory hierarchy.

**Syntax**  
```bash
find [PATH] [OPTIONS] [EXPRESSION]
```

**Examples**  
```bash
find /home/username -name "*.txt"
# Finds all .txt files under /home/username

find . -type d
# Finds all directories in the current directory
```

---

## 14. `man`
**What it does**  
Displays the manual (help) page for a given command.

**Syntax**  
```bash
man COMMAND
```

**Example**  
```bash
man ls
# Opens the manual page for 'ls'
```
> Press `q` to quit.

---

## 15. `which`
**What it does**  
Shows the full path of shell commands.

**Syntax**  
```bash
which COMMAND
```

**Example**  
```bash
which grep
# Might output: /bin/grep
```

---

## 16. `chmod`
**What it does**  
Changes file or directory permissions.

**Syntax**  
```bash
chmod [OPTIONS] MODE FILE...
```

**Examples**  
```bash
chmod u+x script.sh
# Gives the owner (u) execute permission on script.sh

chmod 755 script.sh
# Sets file permissions to rwxr-xr-x
```

---

## 17. `chown`
**What it does**  
Changes file or directory ownership.

**Syntax**  
```bash
chown [OPTIONS] OWNER:GROUP FILE...
```

**Example**  
```bash
sudo chown username:username file.txt
# Changes owner and group of 'file.txt' to 'username'
```

---

## Additional Tips
- **`sudo`**: Use to perform actions requiring administrative privileges, e.g., `sudo apt update`.
- **Tab Completion**: Press `<Tab>` in the terminal to auto-complete commands, file, or directory names.
- **Command History**: Use the Up/Down arrow keys to cycle through previously executed commands.

---

**Practice these commands to get comfortable with the Linux command line.** 
```
