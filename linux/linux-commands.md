# Linux Commands for Cybersecurity

## Introduction
This project contains my Linux command notes for my cybersecurity learning.

## 1. pwd
Displays the current working directory.

```bash
pwd
```


## 2. ls - List Directory Contents
The ls command is used to display files and directories in the current or specified directory.

## Common ls options

## i. ls -a
Displays all files, including hidden files (files starting with a dot).

```bash
ls -a
```
## ii. ls -l
Displays files and directories in long-list format, including permissions, owner, size, and modification date.

```bash
ls -l
```
## iii. ls -R
Displays directory contents recursively, including subdirectories.

```bash
ls -R
```
## iv. ls -al
Displays all files, including hidden files, in long-list format with detailed information like permissions, size, owner, etc.

```bash
ls -al
```
## v. ls -lh
Displays file sizes in a human-readable format (KB, MB, GB).

```bash
ls -lh
```
## vi. ls -t
Sorts files and directories by modification time, newest first.

```bash
ls -t
```


## 3. cd -- Changing Directory command
It changes the current working directory from one directory to another directory.

## i. cd
Takes directly to home directory.

```bash
cd
```
## ii. cd ~
Takes to home directory.

```bash
cd ~
```

## iii. cd ..
Moves one level up to the parent directory.

```bash
cd ..
```

## iv. cd ../..
Moves two directory levels up.

```bash
cd ../..
```

## v. cd /
Takes to the root directory.

```bash
cd /
```
## vi. cd -
Returns to the previous working directory.

```bash
cd -
```


## 4. mkdir - Make Directory
The 'mkdir' command is used to create new directory/folder in linux.

### Common mkdir commands
## i. mkdir directory_name
Its creates a new directory.

```bash
mkdir cybersecurity
```
Then it will create the directory as named cybersecurity.
## ii. To create multiple directory together

```bash
mkdir directory1 directory2 directory3
```
It will create the three directory together.
## iii. Making Parent and Subdirectory together

```bash
mkdir -p cybersecurity/practice
```
Here, -p = option of making parent directory and 
Cybersecurity = parent directory, practice = subdirectory
## iv. Making directory giving with a specific permissions

```bash
mkdir -m 755 directory_name
```
It gives 755 permissions to the directory.

## 5. rmdir - Remove directory
The "rmdir" command is used to remove empty directories.
### Common rmdir commands
## i. rmdir directory_name
Removes empty directory.
```bash
rmdir Practice
```
It removes the practice directory if it is empty.

## ii. rmdir directory1 directory2
Removes multiple directory together.

```bash
rmdir Cyber Practice
```
It removes the two directories cyber and Practice in one command.
## iii. rmdir -r parent_directory/child_directory
Remove specific directory and its parent directory if they are empty.

```bash
rmdir -r CEH/practice
```
Notes: rmdir removes only empty directories. If a directory contains file or other directories, rmdir cannot remove it.


## 6. touch - create a new file
"touch" command is used to create empty files and update file timestamps.

## i. touch file_name
Creates a new file

```bash
touch book.txt
```
It creates an empty file named book.txt in current directory if it doesn't already exist.

## ii. touch file_name1 file_name2
Creates a multiple files

```bash
touch book.txt note.txt
```
It creates two empty file named book.txt and note.txt together.

## iii. touch -c file_name
Updates timestamps only if the file already exists. It does not create a new file.
```bash
touch -c file_name
```

## iv. touch -a file_name
Updates the access time of a file.
```bash
touch -a file_name
```








