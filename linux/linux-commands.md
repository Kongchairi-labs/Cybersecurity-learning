# Linux Commands for Cybersecurity

## Introduction
This project contains my Linux command notes for my cybersecurity learning.

## 1. pwd
Displays the current working directory.

```bash
pwd
```


## 2. ls - List Directory Contents
The 'ls' command is used to display files and directories in the current or specified directory.

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

## 3. cd - Changing Directory command
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
### Common touch commands
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

## 7. cat = Concatenate
The "cat" command is used to display file contents, create files, combine files, and append text to files.
### Common cat commands

## i. cat file_name
Displays the contents of a file.
```bash
cat note.txt
```
It displays the contents of note.txt in terminal.

## ii. cat > file_name
Create and write a file
```bash
cat > note.txt
```
Type the texts, then press Ctrl+D to save and exit. There will be create a file named note.txt and the text will be saved in this file.

Notes: if note.txt is already exists, this overwrite its existing contents.

## iii. cat >> file_name
Type additional text and save
```bash
cat >> note.txt
```
Here we can add texts in note.txt file and save.

## iv. cat file_name file_name
Displays all text together
```bash
cat file1.txt file2.txt
```

## v. cat -n file_name
Displays file contents with line numbers including blank lines.
```bash
cat -n file_name
```

## vi. cat -b file_name
Displays line numbers only for non-empty lines.
```bash
cat -b file_name
```

## vii. cat file1 file2 > file3
Joins two files contents(file1,file2) and stores the output in a new file(file3) 
```bash
cat file_name1 file_name2 > file_name3
```

## less command
The less command allows to read large text files page by page without loading the entire content into terminal display.
### Common less commands

## i. less file_name
The file contents will open on navigation screen.
```bash
less file_name
```
## ii. less -N file_name
Shows contents with line numbers
```bash
less -N file_name
```
## iii. less -S file_name
Prevents long lines from wrapping
```bash
less -S file_name
```

## iv. less +G file_name
Opens at the end of the file
```bash
less +G file_name
```
## v. less -i file_name
Case-insensitive searching
```bash
less -i file_name
```
### Navigation inside "less"
KEY   = FUNCTION, 
Space = Next page, 
b     = Previous page, 
Enter = Next line, 
k     = Previous line, 
g     = Go to beginning, 
G     = Go to end, 
/word = Search for word, 
n     = Previous search match, 
q     = Quit.


## 7. "head" command in Linux
The head command displays the beginning (first lines) of a file.
By default, it displays the first 10 lines of a file.
### Common 'head' commands

## i. head file_name
It displays the first 10 lines of that file.
```bash
head lab.txt
```
This displays the first 10 lines of lab.txt.

## ii. head -n 5 file_name
It displays the first 5 lines of the file.
```bash
head -n 5 library.txt
```
It displays the first 5 lines of library.txt file.

## iii. head -n 10 file_name1 file_name2
It displays the first 10 lines of both two files.
```bash
head -n 20 note.txt book.txt
```
Note : 'n' = number of lines to display

## iv. head -c 50 file_name
It displays first 50 bytes of the file
```bash
head -c 50 poem.txt
```
It displays the first 50 bytes of poem.txt file.
Note: 'c' = number of sizes to display

## v. head -q file_name1 file_name2
Hides filenames when displaying multiple files
```bash
head -q file_name1 file_name2
```

## vi. head -v file_name1 file_name2
Always displays the filename header
```bash
head -v file_name1 file_name2
```


## 9. "tail" command in Linux
The head command displays the last lines of a file.
By default, it displays the last 10 lines of a file.

### Common 'tail' commands
## i. tail notes.txt
It displays the last 10 lines of notes.txt file.
```bash
tail notes.txt
```
## ii. tail -n 5 notes.txt
It displays the last 5 lines of notes.txt file.
```bash
tail -n 5 notes.txt
```
## iii. tail -c 20 notes.txt
It displays the last 20 bytes of notes.txt file.
```bash
tail -c 20 notes.txt
```
### iv. tail -f filename
Its Continuously monitors new content
```bash
tail -f filename
```
This displays new lines as they are added to the log file.
Press Ctrl + C to stop monitoring.

## v. tail -q filename1 filename2
Hides filename headers
```bash
tail -q filename1 filename2
```

## vi. tail -v filename1 filename2
Always displays filename headers
```bash
tail -v filename1 filename2
```





