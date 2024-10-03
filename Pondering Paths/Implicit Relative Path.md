# Implicit Relative Paths, form /
## EXPLANATION 
The eigth task was to to run `/challenge/run`  while having a current working directory of `/challenge` by using the implicit entry`.`.
It required me to change my directory to `/challenge` using the `cd` and the excute `run` program using the implicit entry.
so i changed my directory to `/challenge` using the `cd` and then i typed `./run` in the terminal which was equal to the command `/challenge/run` .
Then i copy pasted the generated flag into the `pwn.college` site.
## CODE 
```bash
Connected!
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{IR-aa1a_r21W3o2Ew28ZN0s8nsg.dFTN1QDL4YDN0czW}
```
## RESOURCES 
none 
