### Linux File-Management commands

## cp - Copy
The command "cp" is used to copy files and directories from one locatiin to another.
### Common "cp" commands
## i. cp source_file destination_file
Copy a file from source file to destination file keeping the source file unchanged.
```bash
cp file.txt backup.txt
```
All the contents in file.txt will be copied into backup.txt.

## ii. cp source_file directory
Copy a file from a source file to a directory.
```bash
cp file.txt Documents/
```
Its copy all the contents of file.txt to Documents directory.

## iii. cp file1 file2 directory
Copy multiple files into a directory
```bash
cp file1_name file2_name directory
```

## iv. cp -r = Copy directories
Copy a directory and everything inside it into another directory.
```bash
cp -r directory1 directory2
```
This copies directory1 and its contents into a new directory named directory2 (if directory2 does not already exist).

## v. cp -i = Interactive copying
The -i option asks for confirmation before overwriting an existing file
```bash
cp -i note.txt pdf.txt
```
If pdf.txt already exists, Linux asks whether you want to overwrite it or not.

## vi. cp -n = Do not overwrite
The -n options prevents an existing destination file from being overwritten.
```bash
cp -n note.txt pdf.txt
```
If pdf.txt already exists, it remains unchanged.








