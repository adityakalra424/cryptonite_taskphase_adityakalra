# Learning Complex Usage
## INTRODUCTION 
In the 2nd challenge, we have to read the documentation and get the flag 
DOCUMENTATION:Welcome to the documentation for /challenge/challenge! This program allows you to print arbitrary files to the terminal, when given the `--printfile `argument.
The argument to the --printfile argument is the path of the flag to read. For example, /challenge/challenge --printfile /challenge/DESCRIPTION.md will print out the description of the level!
The documentation tell us how to use the /challenge/challenge program.The command to use the program is `/challenge/challenge --printfile /flag ` where `/challenge/challenge` is a command 
`--printfile` is a argument and the file path `/flag` is also an argument. This command prints  any file that is mentioned after `--printfile`.
## CODE
```bash
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /flag
Correct argument! Here is the /flag file:
pwn.college{MXKS98lxEy6EZDb1Ne7Enr5NF01.dFzN1QDLxMDO1czW}
```
# RESOURCES 
none 
