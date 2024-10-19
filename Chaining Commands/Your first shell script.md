# Your first shell script
## INTRODUCTION
In the 2nd challenge, we have to create a shell script called `x.sh` which will excuted the commands `/challenge/pwn` and then `/challenge/college` which will get me the flag. I typed `nano x.sh` ( `nano` is a simple, command-line based editor) to create a shell script named `x.sh`.THIS RESULTED IN OPENING A COMMAND LINE BASED EDITOR WITH A FILE NAMES `x.sh` . In the `x.sh` file i added a `shebang line` `#!/bin/bash` which specifies which interpreter should be used to run the script which is `bash` and then i added the commands `/challenge/pwn` and then `/challenge/college` and then i saved the file and exited the editor.After that i wrote `bash x.sh` in the terminal to run the file using `bash`.Then i got the file.
## CODE
```bash
Connected!                                                                        
hacker@chaining~your-first-shell-script:~$ nano x.sh
hacker@chaining~your-first-shell-script:~$ bash x.sh
Great job, you've written your first shell script! Here is the flag:
pwn.college{4OPE0mK6nxL_O2o9nUsjYLwfIrx.dFzN4QDL4YDN0czW}
```
## RESOURCES
[google ](https://www.geeksforgeeks.org/how-to-create-a-shell-script-in-linux/)
leo ai


