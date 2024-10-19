# Adding commands
## INTRODUCTION
In the 3rd challenge,we had to create a command `win` which cat `/flag` to get the flag.I wrote `echo $PATH` to find the absolute path of the `cat` command.then i wrote
`nano win` to create a shell script named `win` in the home directory then i wrote `cat /flag` in the `win` shell script and saved it , then i wrote `chmod ugo+rwx win` to make it excutable, then i defined the `PATH` variable by writing 
`PATH=/home/hacker:/bin:/usr/bin` (the `cat` command was in `/bin`) , then i ran `/challenge/run` to get the flag.
## CODE
```bash
Connected!
hacker@path~adding-commands:~$ echo $PATH
/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
hacker@path~adding-commands:~$ nano win
hacker@path~adding-commands:~$ chmod ugo+rwx win
hacker@path~adding-commands:~$ PATH=/home/hacker:/bin:/usr/bin
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{8-EH_58cKs9l92_UZG721BY2jSn.dZzNyUDL4YDN0czW}
```
## RESOURCES
none
## REMARK
i did check all the paths in the `PATH` VARIABLE TO FIND THE `cat` command i just didnt include the lines for that in the code.
