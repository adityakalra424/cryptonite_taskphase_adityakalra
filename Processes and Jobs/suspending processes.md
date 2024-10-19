# suspending processes
## INTRODUCTION 
In the 4th challenge we learn how to suspend processes to the background with `Ctrl-Z`.In this challenge
we have to Use the terminal to launch `/challenge/run`, then suspend it, then launch another copy while the first is suspended to get the flag.
so I wrote `/challenge/run` to launch it, then i pressed `Ctrl-Z` to suspend it, then i wrote `/challenge/run` to launch another copy and then i got the flag.
## CODE
```bash
Connected!
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          82      65  0 10:21 pts/0    00:00:00 bash /challenge/run
root          84      82  0 10:21 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          82      65  0 10:21 pts/0    00:00:00 bash /challenge/run
root          89      65  0 10:21 pts/0    00:00:00 bash /challenge/run
root          91      89  0 10:21 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{ITmUSQsa652J2MVXgkgN1vb2DsY.dVDN4QDL4YDN0czW}
```
## RESOURCES
none
