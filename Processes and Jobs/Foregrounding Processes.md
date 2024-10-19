# Foregrounding Processes
## INTRODUCTION
In the 7th challenge, we had to suspend `/challenge/run`, resume the suspended process in the
background, and then foreground it without re-suspending it.So i typed `/challenge/run` to envoke it then I pressed `crtl+z` to suspend the process `/challenge/run` and i wrote `bg /challenge/run` to resume the suspended process in the background using the `bg` command. Then i wrote `fg /challenge/run` to foreground the process directly from the background.Then i got the flag.
## CODE
```bash
Connected!
hacker@processes~foregrounding-processes:~$ /challenge/run
To pass this level, you need to suspend me, resume the suspended process in the
background, and *then* foreground it without re-suspending it! You can
background me with Ctrl-Z (and resume me in the background with 'bg') or, if
you're not ready to do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~foregrounding-processes:~$ bg /challenge/run
[1]+ /challenge/run &



Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out. After that, resume me into the foreground with 'fg';
I'll wait.
hacker@processes~foregrounding-processes:~$ fg /challenge/run
/challenge/run
YES! Great job! I'm now running in the foreground. Hit Enter for your flag!

pwn.college{I3DU-vU2Ligzse49mrJbe4d9tKo.dhDN4QDL4YDN0czW}
```
## RESOURCES
none
