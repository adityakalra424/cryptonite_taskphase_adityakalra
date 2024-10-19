# Redirecting script output
## INTRODUCTION
In the 3rd challenge, we have to create a shell script which contains the commands `/challenge/pwn` command followed by the `/challenge/college` command and then redirect the output of the shell script into the input of `/challenge/solve` using piping `|` to get the flag.I wrote `nano x.sh` to create a shell script named `x.sh` and open it in a text editor.Then i wrote `#!/bin/bash /challenge/pwn /challenge/college` and saved the file. Then i wrote `bash x.sh | /challenge/solve`
where `bash` excutes the `x.sh` shell script and the `|` pipes the output of `bash x.sh` into the input of `/challenge/solve`.Then i get the flag.
## CODE
```bash
connected!                                                                        
hacker@chaining~redirecting-script-output:~$ nano x.sh
hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{8m5P48T6MoRQbVkpxxe9R7iDpzK.dhTM5QDL4YDN0czW}
```
## RESOURCES
none
