# Grepping errors 
## INTRODUCTION 
In the 8th challenge, we have to learn how to grep through errors using `>& ` operator.So first we have to redirect standard error to standard output using `2>&1` and 
then pipe the now-combined stderr and stdout as normal using  `|`.I wrote `/challenge/run 2>&1 | grep pwn.college` where `2>&1` redirects the standard error of `/challenge/run` to standard output
and pipe the comnined output using  the `|` operator and then grep throught the strout and strandard error to find the flag.
## CODE
``` bash
Connected!
hacker@piping~grepping-errors:~$ /challenge/run 2>&1 | grep pwn.college
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stderr : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stderr to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/xpq4yhadyhazkcsggmqd7rsgvxb3kjy4-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stderr!
[PASS] Success! You have satisfied all execution requirements.
pwn.college{QxIwSYBxaxDIWPL_kieAUlXUktt.dVDM5QDL4YDN0czW}
```
## RESOURCES
none
