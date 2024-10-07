# Making Directories
## Introduction 
In the tenths task, we had to create a directory using the `mkdir` command and then create a file using the `touch` command. I created a directory named `/tmp/pwn` 
using the `mkdir` command and then i `cd` to that directory and then i created a file using the `touch` command.
after solving the challenge, i copy pasted the generated flag in the `pwn.college` site.

## CODE
``` bash
Connected!
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ touch college
hacker@commands~making-directories:~$ /challenge/run
Uh oh! /tmp/pwn/college does not exist. Please use the 'touch' command to
create it!
hacker@commands~making-directories:~$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{ITadzvcJxEFkIKq2E4mqI1RhIRL.dFzM4QDL4YDN0czW}
```
## RESOURCES 
none
