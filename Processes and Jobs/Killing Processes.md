# Killing Processes
## INTRODUCTION 
In the 2nd challenge,we learn how to kill a process using the `kill` command.You use `kill` to
terminate it by passing the process identifier  as an argument.In this challenge we had to `kill`
`/challenge/dont_run` before running `/challenge/run` to get the flag.I wrote `ps -ef` to get the list
of running programs and then i killed the `/challenge/dont_run` using the `kill 73` where `kill` is 
the command and `73` is the process identifies of the process as an argument.Then i ran `/challenge/run`
to get the flag.
## CODE
``` bash
Connected!
hacker@processes~killing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 10:02 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/default/b
root           7       1  0 10:02 ?        00:00:00 /run/dojo/bin/sleep 6h
root          71       1  0 10:02 ?        00:00:00 su -c /challenge/.launcher hacker
hacker        73      71  0 10:02 ?        00:00:00 /challenge/dont_run
hacker        74      73  0 10:02 ?        00:00:00 sleep 6h
hacker        75       0  0 10:02 pts/0    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker        92      75  0 10:02 pts/0    00:00:00 ps -ef
hacker@processes~killing-processes:~$ kill 73
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{oMS-YB6btxdaDz_gzS-qyzUfdcf.dJDN4QDL4YDN0czW}
```
## RESOURCES
none
