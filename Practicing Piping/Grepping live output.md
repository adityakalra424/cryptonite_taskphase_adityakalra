# Grepping live output
## INTRODUCTION 
In the 7th challenge we have to learn to use the `| (pipe)` `operator`Standard output from the command to the left of the pipe will be connected to (piped into) the standard input of the command to the right of the pipe.
I wrote `/challenge/run | grep pwn.college` in the command line.The `/challenge/run` output was piped into `grep pwn.college` using the `|` operator  and the `grep` command grep from the output of `/challenge/run` the txt that had `pwn.college` which is the flag.
## CODE 
```bash
adityakalra@DESKTOP-BBS45RH:~$ ssh -i./key hacker@dojo.pwn.college
Connected!
hacker@piping~grepping-live-output:~$ /challenge/run | grep pwn.college
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stdout : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/xpq4yhadyhazkcsggmqd7rsgvxb3kjy4-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stdout!
[PASS] Success! You have satisfied all execution requirements.
pwn.college{Y77geEcyz0-aBEM1Ez7Yfkpz8_r.dlTM4QDL4YDN0czW}
```
## RESOURCES
none
