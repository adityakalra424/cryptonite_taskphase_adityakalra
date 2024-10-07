# Mixing Globs 
## INTRODUCTION 
In the 5th challenge, We have to `cd` to `/challenge/files` and, using the globbing you've learned,
write a single, short (6 characters or less) glob that will match the files "challenging", "educational", and "pwning".
This can be done by writing the arguement as `[cep]*` where the `[]` implies that the first character can be `c,e,p` and the rest of the characters can be anything because the whole list of files 
contain only one word starting with `e` that is `educational`, only one word starting with `c` that is `challenging` and only on word starting with `p` which is `pwning`.
## CODE 
```BASH
Connected!
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ ls
amazing      delightful   great       jovial    magical     pwning   splendid   victorious  youthful
beautiful    educational  happy       kind      nice        queenly  thrilling  wonderful   zesty
challenging  fantastic    incredible  laughing  optimistic  radiant  uplifting  xenial
hacker@globbing~mixing-globs:/challenge/files$ echo look: *[ing]
look: amazing challenging laughing pwning thrilling uplifting
hacker@globbing~mixing-globs:/challenge/files$ [ed]*ing
ssh-entrypoint: [ed]*ing: command not found
hacker@globbing~mixing-globs:/challenge/files$ echo look: [ed]*ing
look: [ed]*ing
hacker@globbing~mixing-globs:/challenge/files$ echo look: [cep]*ing
look: challenging pwning
hacker@globbing~mixing-globs:/challenge/files$ echo lokk: [cep]*
lokk: challenging educational pwning
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{4Eoy1FzYo966JZ1FU_0VE-wEK3a.dVjM4QDLxMDO1czW}
```
## RESOURCES 
none
