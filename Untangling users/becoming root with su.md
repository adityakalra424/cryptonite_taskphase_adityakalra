# Becoming root with su
## INTRODUCTION
In the 1st challenge,we have to use `su` command to become `root` but to become `root` we have to provide a password to `su` which is `hack-the-planet` and then cat `/flag` to get the flag.I wrote `su` then i typed the password `hack-the-planet` which made me `root` then i typed `cat /flag` to get the flag.
## CODE
```bash
Connected!
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# /flag
bash: /flag: Permission denied
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{ALcKph3znHgnsAWMPzAvItvp0gX.dVTN0UDL4YDN0czW}
```
## RESOURCES
none
