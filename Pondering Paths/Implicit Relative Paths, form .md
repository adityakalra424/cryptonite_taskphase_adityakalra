# Implicit Relative Paths, form /
## EXPLANATION 
The sixth task was to to run `/challenge/run` using a relative path while having a current working directory of `/`.
It required me to execute the `/challenge/run` program from a specific path (which it will tell me).
So i first i executed the `/challenge/run` to find from which directory i had to execute the `/challenge/run` program from.
Then i `cd` to that directory and typed  `challenge/run` in the terminal which was the relative path to `run` program .Then i copy pasted the generated flag into the `pwn.college` site.
## CODE 
```bash
hacker@paths~implicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the cd utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ /challenge/run
Incorrect...
You invoked this challenge with an absolute path. This challenge needs a relative path!
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{gNxe27yDB5XS557nE9uazPzXTtL.dlDN1QDL4YDN0czW}
```
## RESOURCES 
none 
