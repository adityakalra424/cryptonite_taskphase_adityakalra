# Groups and Files
## INTRODUCTION
In the 2nd challlenge we learn about the groups and the use of the `chgrp` (change group) command.
In this challenge we had to change the group of the `/flag` file to the `hacker` group,and then get the flag.I wrote `chgrp hacker /flag` to change the group of the `/flag` file and then i `cat` it to get the flag.
## CODE
```bash
Connected!
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{gsdBRm3SOC3-KcoVeU39B6ltQ_p.dFzNyUDL4YDN0czW}
```
## RESOURCES
none
