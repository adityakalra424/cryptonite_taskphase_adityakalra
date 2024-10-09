# Duplicating piped data with tee
## INTRODUCTION 
In the 9th challenge, we have to duplicate the piped date using the `tee` command. In this challenge  `/challenge/pwn` must be piped into `/challenge/college`, but we will need to intercept the data to see what pwn needs using the `tee` command.
I wrote `/challenge/pwn | tee file | /challenge/college` where `/challenge/pwn` output is duplicated into `file` file to debug it.Then i `cat` the file `file` to find the correct conditions to use `/challenge/pwn`.
Then i solved it to get the flag.
## CODE
``` bash
Connected!
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee file | /challenge/college
Processing...
WARNING: you are overwriting file file with tee's output...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat file
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "ETWnfjTE"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret ETWnfjTE | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{ETWnfjTEOT7Ow8eorQQiW-Su4ow.dFjM5QDL4YDN0czW}
```
## RESOURCES 
none
