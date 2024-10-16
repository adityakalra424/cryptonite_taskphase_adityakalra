# Changing File ownership
## INTRODUCTION 
In the 1st challlenge we learn about the file ownership and the use of the `chown` (change owner) command.In this challenge we had to change
the owner of the `/flag` file to the hacker user, and then get the flag.I wrote `chown hacker /flag` to change the owner of the `/flag` file and then i `cat` it to get the flag.
## CODE
```bash
Connected!
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{MxLn29cmTNCrcadE6JTEhwu3nYR.dFTM2QDL4YDN0czW}
```
## RESOURCES
none
