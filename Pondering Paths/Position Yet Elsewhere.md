# Position Yet Elsewhere
## EXPLANATION 
The fifth task was to navigate around directories by using the cd (change directory) command and pass a path to it as an argument.
It required me to execute the `/challenge/run` program from a specific path (which it will tell me).
So i first i executed the `/challenge/run` to find from which directory i had to execute the `/challenge/run` program from.The directory was `/var`directory
Then i `cd` to `/var` directory and reexecuted the `/challenge/run` program.Same as fourth task.Then i copy pasted the generated flag into the `pwn.college` site.
## CODE 
```bash
Connected!
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /var directory.
Please use the cd utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /var
hacker@paths~position-yet-elsewhere:/var$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{Yq3M3T-xcQqGdlM_hQ0kJe5-7P3.dhDN1QDL4YDN0czW}
```
## RESOURCES 
none 
