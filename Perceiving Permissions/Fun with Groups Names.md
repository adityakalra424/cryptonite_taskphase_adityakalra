# Fun with Groups Names
## INTRODUCTION
In the 3rd challenge, we had to cat `/flag` but the name of the group in which `hacker` belonged to was randomized.So i wrote `id` to find in which group did the hacker user belonged to which was ` groups=1000(grp14147)`.
Then i wrote `chgrp grp14147 /flag` to change the group of `/flag` file to `grp14147` so that i could `cat` it. Then i `cat` the `/flag` file to get the flag.
## CODE
```BASH
Connected!
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp14147) groups=1000(grp14147)
hacker@permissions~fun-with-groups-names:~$ chgrp grp14147 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{w3G-dJZaaYo8it8OLr_on3vWL0D.dJzNyUDL4YDN0czW}
```
## RESOURCES
none
