# Position Elsewhere
## EXPLANATION 
The fourth task was to navigate around directories by using the `cd` (change directory) command and pass a path to it as an argument.
It required me to execute the `/challenge/run` program from a specific path (which it will tell me).
So i first i executed the `/challenge/run` to find from which directory i had to execute the `/challenge/run` program from.That directory was `/sys`
Then i `cd` to `/sys` and reexecuted the `/challenge/run` program.Same as the third task.Then i copy pasted the generated flag into the `pwn.college` site.
## CODE 
```bash
Connected!
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /sys directory.
Please use the cd utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /sys
hacker@paths~position-elsewhere:/sys$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{waCixLt8kWzljtPljN2RspDf4xV.ddDN1QDL4YDN0czW}
```
## RESOURCE 
none 
