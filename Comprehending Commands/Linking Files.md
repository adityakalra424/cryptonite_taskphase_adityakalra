# Linking Files 
## INTRODUCTION 
In the 12th challenge, the flag is, as always, in /flag, but /challenge/catflag will instead read out /home/hacker/not-the-flag.
we had to use the symlink, and fool it into giving you the flag.I linked `/flag` with `/home/hacker/not-the-flag` using the `ln -s` command.Then ran the `/challenge/catflag` command to read the `/home/hacker/not-the-flag` which will point to the `/flag `file.

## CODE 
```bash
hacker@commands~linking-files:/challenge$  cd ~
hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{AZgEmPRUSPBdSMpsu77YgqnESWz.dlTM1UDLxMDO1czW}
```
## RESOURCES 
none
