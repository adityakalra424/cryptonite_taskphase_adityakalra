# Starting background processes
## INTRODUCTION
In the 8th challenge, we learn how to background a process right off the bat using the `&` argument.I wrote `/challenge/run &` to start the `/challenge/run` process
directly in the background with the help of `&`.Then i got the flag.

## CODE
```bash 
Connected!
hacker@processes~starting-backgrounded-processes:~$ /challenge/run &
[1] 82
hacker@processes~starting-backgrounded-processes:~$


Yay, you started me in the background! Because of that, this text will probably
overlap weirdly with the shell prompt, but you're used to that by now...

Anyways! Here is your flag!
pwn.college{ck_MfZguNEe_O8_G_MFxx34ddPR.dlDN4QDL4YDN0czW}

[1]+  Done                    /challenge/run
```
## RESOURCES
none
