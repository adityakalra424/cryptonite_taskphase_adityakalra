# Process Exit Code
## INTRODUCTION
In the 9th challenge,we learn about exit codes and how to retrieve them.In this challenge we had to retrieve the exit code returned by `/challenge/get-code`
and then run `/challenge/submit-code` with that error code as an argument.I wrote `/challenge/get-code` to run the process and then i wrote `echo $?` to print the error code 
onto the terminal using the `echo` command and `?` command which was `28`. then i wrote `/challenge/submit-code 28` to finish the challenge and get the flag.
## CODE
``` bash
Connected!
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
28
hacker@processes~process-exit-codes:~$ /challenge/submit-code 28
CORRECT! Here is your flag:
pwn.college{MA9h4qqFBmEaVhq-87OqIjNmc8w.dljN4UDL4YDN0czW}
```
## RESOURCES
none
