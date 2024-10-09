# Redirecting Inputs
## INTRODUCTION 
In the 5th challenge, we have to learn how to redirect inputs using `<`.In this challenge we had to have the `PWN` file contain the value `COLLEGE` and redirect the `PWN` file to
`/challenge/run` using `<`. Firstly i wrote `echo COLLEGE > PWN` to redirect the output of `echo COLLEGE`  to the `PWN` file(`PWN` file contains the value `COLLEGE`)
Then i wrote `/challenge/run < PWN` to redirect my input into `/challenge/run`.Then i got the flag.
## CODE
``` bash
Connected!
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{EZA39qKniCA1tVhKxq-GeyXNuNv.dBzN1QDL4YDN0czW}
```
## RESOURCES
none
