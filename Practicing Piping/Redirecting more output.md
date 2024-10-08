# Redirecting more outputs
## INTRODUCTION 
In the 2nd challenge, we have to redirect the output of `/challenge/run` to the file `myflag`.The flag will then end up in `myflag`.So we can use `cat` to get the file content and thus get the file.
I typed `/challenge/run > myflag` where `>` redirects the output of `/challenge/run` to the file `myflag` and then i typed `cat myflag` to get the flag.

## CODE 
``` BASH
Connected!
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{M09JmLEME01efj1J-sF8NqD89fg.dVjN1QDL4YDN0czW}
```
## RESOURCES 
none
