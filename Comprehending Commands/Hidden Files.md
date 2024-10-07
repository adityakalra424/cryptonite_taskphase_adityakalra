# Hidden Files
## INTRODUCTION 
In the eigth challenge, we had to view the hidden files in the `/` using the `ls -a`. 
Then `cat` the hidden file to get the flag. After solving the challenge, i copy pasted the generated flag in the `pwn.college` site. 

## CODE
```bash
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv           bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-3222414509777  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-322241509777
cat: .flag-322241509777: No such file or directory
hacker@commands~hidden-files:/$ cat .flag-3222414509777
pwn.college{sj2GXEHntnNq0akJP12UkukrK5M.dBTN4QDLxMDO1czW}
```
## RESOURCES 
none

