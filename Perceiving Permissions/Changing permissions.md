# Changing permissions
## INTRODUCTION 
In the 4th challenge we learn the use of `chmod`(change mode) command.In this challenge we had to change the permission of the `/flag` file to read it.I wrote `chmod ugo+rwx /flag`
to change the permission of `/flag` where the user`u` ,group`g` and other`o`can read`r`, write`w` and excute`x` the file.Then i `cat` the file to get the flag. 
## CODE
``` BASH
hacker@permissions~changing-permissions:~$ chmod ugo+rwx /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{0O7NLqxEK2wzMYVJKivas73oN4l.dNzNyUDL4YDN0czW}
```
## RESOURCES
none
