# Backgrounding Processes
## INTRODUCTION 
In the 6th challenge, we learn how to resume processes in the background with the `bg` command.
This will allow the process to keep running, while giving me my shell back to invoke more commands in the meantime.
In this challenge we had to Use the terminal to launch `/challenge/run`, then suspend it,
then background it with `bg` command and then  launch another copy while the first is running in the background!.
I wrote `/challenge/run` to launch the process, then i pressed`crtl+z` to suspend it, then i wrote `bg /challenge/run` to resume the process in the background
and then i again resumed the process.Then i got the flag.
## CODE
```bash
Connected!
hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root          82 S+   bash /challenge/run
root          84 R+   ps -o user=UID,pid,stat,cmd

I don't see a second me!

To pass this level, you need to suspend me, resume the suspended process in the
background, and then launch a new version of me! You can background me with
Ctrl-Z (and resume me in the background with 'bg') or, if you're not ready to
do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~backgrounding-processes:~$ bg /challenge/run
[1]+ /challenge/run &



hacker@processes~backgrounding-processes:~$ Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out.

hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root          82 S    bash /challenge/run
root          92 S    sleep 6h
root          93 S+   bash /challenge/run
root          95 R+   ps -o user=UID,pid,stat,cmd

Yay, I found another version of me running in the background! Here is the flag:
pwn.college{s8Y-icfWo_YGP6sWASNZ1yTKQ38.ddDN4QDL4YDN0czW}
```
## RESOURCES
none
