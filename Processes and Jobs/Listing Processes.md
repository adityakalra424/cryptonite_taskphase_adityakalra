# Listing Processes
## INTRODUCTION 
In the 1st challenge, we have to find the `/challenge/run` which is renamed to a random filename
but it is a running program. We can find the program by using the `ps` command which lists all 
the running programs.So i wrote `ps -ef` to list out all the running programs and 
then i found `/challenge/11041-run-5441` which is `/challenge/run` just in a different name.
Then i ran the program to get the flag.
## CODE
``` bash
Connected!
hacker@processes~listing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 09:51 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/default/b
root           7       1  0 09:51 ?        00:00:00 /run/dojo/bin/sleep 6h
root          68       1  0 09:51 ?        00:00:00 /challenge/11041-run-5441
root          72      68  0 09:51 ?        00:00:00 sleep 6h
hacker        73       0  0 09:51 pts/0    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker        90      73  0 09:52 pts/0    00:00:00 ps -ef
hacker@processes~listing-processes:~$ /challenge/11041-run-5441
Yahaha, you found me! Here is your flag:
pwn.college{MIdQNoZiwGMS_UBwHQzzXtWaRbI.dhzM4QDL4YDN0czW}
Now I will sleep for a while (so that you could find me with 'ps').
```
## RESOURCES
none
