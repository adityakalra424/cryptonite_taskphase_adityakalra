# Writing to multiple programs
## INTRODUCTION 
In the 10th challenge, we have to Run the `/challenge/hack` command, and duplicate its output as input to both the `/challenge/the` and the `/challenge/planet` commands
So i wrote `/challenge/hack | tee >(/challenge/the) >(/challenge/planet)` to duplicate its output to both the `/challenge/the` and the `/challenge/planet` commands.

##CODE
``` BASH
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
175137101271523582
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{II-T8LUjVmmkoYd_gYUbw4HqzAJ.dBDO0UDL4YDN0czW}
```
## RESOURCES 
google search process substitution 
