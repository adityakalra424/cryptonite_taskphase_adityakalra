# Executable file
## INTRODUCTION 
In 5th challenge, we had to change the permission of the `/challenge/run` program so that the user which is the `hacker` can excute the file using `chmod`.
So i wrote `chmod u+x /challenge/run`to change the permission so that the user (`u`) could excute (`x`) the program `/challenge/run`.
Then i excuted the program to get the flag.
## CODE
```BASH
hacker@permissions~executable-files:/$ chmod u+x /challenge/run
hacker@permissions~executable-files:/$ /challenge/run
Successful execution! Here is your flag:
pwn.college{I9yxF1QWYLcR2eOb2m-5Wt1SsLh.dJTM2QDL4YDN0czW}
```
## RESOURCES
none
