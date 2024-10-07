# Listing Files 
## INTRODUCTION 
In the fifth challenge, we have to list the files in `/challenge` to find the file `/challenge/run` which is in another name.
To solve this,I `cd` to `/challenge`, then i used the `ls` command to list out the files in `/challenge`.File `11876-renamed-run-20880` was one of the files in `/challenge`
Then i ran `/challenge/11876-renamed-run-20880` in the command line to get the flag.

## CODE
``` bash
Connected!
hacker@commands~listing-files:~$ cd /challenge
hacker@commands~listing-files:/challenge$ ls
11876-renamed-run-20880  DESCRIPTION.md
hacker@commands~listing-files:/challenge$ /challenge/11876-renamed-run-20880
Yahaha, you found me! Here is your flag:
pwn.college{QLTp9H3St8poDXxQ1Af7HrXO1EV.dhjM4QDLxMDO1czW}
```
## RESOURCES 
none
