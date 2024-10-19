# Reading Files
## INTRODUCTION 
In the 8th challenge,we have to read `/challenge/read_me` into the `PWN` environment variable.
So i wrote `read PWN</challenge/read_me` where the output of `/challenge/read_me` is redirected to the input of `PWN`.Then the `read` command reads into `PWN`.
Then we get the flag for the challenge.
## CODE
``` bash
hacker@variables~reading-files:~$ read PWN</challenge/read_me
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{YmWYInQu7vF7J1rYpkVMMI8_ChZ.dBjM4QDL4YDN0czW}
```
## RESOURCES
none

