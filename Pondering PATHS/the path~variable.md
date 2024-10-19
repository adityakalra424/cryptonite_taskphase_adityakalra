# the path variable
## INTRODUCTION
In the 1st challenge, we learn about special shell variable called `PATH`, that stores a bunch of directory paths in which the shell will search for programs corresponding to commands.In this challenge we have disrupt the operation of the `/challenge/run` program. This program will `DELETE` the flag file using the `rm` command. However, if it can't find the `rm` command, the flag will not be deleted, and the challenge will give it to you! Thus, we must make it so that `/challenge/run` also can't find the `rm` command.I wrote `PATH=""` to make the `PATH` variable blank so that when i run the `/challenge/run` it wont be able to find the `rm` command which will not result in deletion of the flag.
## CODE
```bash
Connected!                                                                        
hacker@path~the-path-variable:~$ PATH=""
hacker@path~the-path-variable:~$ ls
ssh-entrypoint: ls: No such file or directory
hacker@path~the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{0I65WNug9joqMgKS888_d6ipPMj.dZzNwUDL4YDN0czW}
```
## RESOURCES
none
