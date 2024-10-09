# Redirecting errors
## INTRODUCTION 
In the 4th challenge,you will need to redirect the output of `/challenge/run` to `myflag`, and the `errors` (in our case, the instructions) to the `instructions` file.
Using `>` and `2>`.
I wrote `/challenge/run > myflag 2> instructions` where  `>` redirects the output of `/challenge/run` to `myflag` and `2>` redirects the error to `instructions`.

## CODE
``` BASH
hacker@piping~redirecting-errors:~$ /challenge/run > myflag 2> instructions
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{of0zdKlwxYvSDtRqhz9IlIInM7y.ddjN1QDL4YDN0czW}
```
## RESOURCES 
none

