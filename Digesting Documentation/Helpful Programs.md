# Helpful Programs
## INTRODUCTION 
In the 5th challenger, we have to use the `--help` argument to read a program's documentation when it doesnt have a man page and find how to use the program correctly to print the flag.
## CODE 
``` bash
Connected!
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 41
hacker@man~helpful-programs:~$ /challenge/challenge -g 41
Correct usage! Your flag: pwn.college{0mX4r1RUDnI4l4BB4fpBjthbPug.ddjM4QDLxMDO1czW}
```
## RESOURCES 
none
