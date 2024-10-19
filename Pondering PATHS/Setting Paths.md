# Setting Paths
## INTRODUCTION
In the 2nd challenge, we have write the path of the `win` which is `/challenge/more_commands` in the `PATH` varible because in order to get the flag we need to run `/challenge/run` which will run the `win` command and its path is not in the `PATH` varible so we need to write it manually.I wrote  `PATH=/challenge/more_commands`
to write the path of `win` command in the `PATH` variable. Then i wrote `/challenge/run` to get the flag.
## CODE
```BASH
Connected!                                                                        
hacker@path~setting-path:~$ PATH=/challenge/more_commands
hacker@path~setting-path:~$ /challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{8TTc8z-cpntWKKG0OKa_CGip9ql.dVzNyUDL4YDN0czW}
```
## RESOURCES
none
