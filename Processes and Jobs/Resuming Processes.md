# Resuming Processes
## INTRODUCTION 
In the 5th challenge, we learn how to resume suspended processes using the `fg` command.Tn this challenge we had to suspend `/challenge/run` then resume it using `fg` command.
I wrote `/challenge/run` to start the process then i pressed `Ctrl-Z` to suspend the process and then i wrote `fg /challenge/run` to resume the process and then i got the flag.

## CODE
```bash
Connected!
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$
hacker@processes~resuming-processes:~$ fg /challenge/run
/challenge/run
I'm back! Here's your flag:
pwn.college{8qzdHfgE3XLSut9VzL6fB6qejQm.dZDN4QDL4YDN0czW}
Don't forget to press Enter to quit me!

Goodbye!
```
## RESOURCES
none
