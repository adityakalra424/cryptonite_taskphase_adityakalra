# Storing command output
## INTRODUCTION 
In the 6th challenge,we learn something called `command substitution`, in this challenge we have to read the output of the `/challenge/run` command directly into a variable called `PWN`, and read that variable because it will contain the flag.
So i wrote `PWN=$(/challenge/run)` to read the output of the `/challenge/run` command directly into a variable called `PWN`. then i wrote `echo $PWN` to print the content of the variable `PWN` and get the flag.
## CODE
```bash
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{Q3dANufIMiolNxMaK48g6eYTUba.dVzN0UDL4YDN0czW}
```
## RESOURCES
none
