# Implicit Relative Paths, form /
## EXPLANATION 
The seventh task was to to run `/challenge/run` using a relative path while having a current working directory of `/` and use the implicit entries.
It required me to execute the `/challenge/run` program from a specific path (which it will tell me).
So i first i executed the `/challenge/run` to find from which directory i had to execute the `/challenge/run` program from.
Then i `cd` to that directory and typed  `./challenge/run` in the terminal which was the relative path to `run` program using the implicit entry.
Then i copy pasted the generated flag into the `pwn.college` site.
## CODE 
```bash
Connected!
hacker@paths~explicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ /challenge/run
Incorrect...
You invoked this challenge with an absolute path. This challenge needs a relative path!
hacker@paths~explicit-relative-paths-from-:/$ challenge/run
Incorrect...
This challenge must be called with a relative path that explicitly starts with a `.`!
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{gG_CqTq75dDW6BliDJMDZHfqzT8.dBTN1QDL4YDN0czW}
```
## RESOURCES 
none 
