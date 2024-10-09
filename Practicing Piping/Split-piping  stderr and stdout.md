# Split-piping  stderr and stdout
## INTRODUCTION 
In the 11th challenge, we have to redirect hack's stderr to `/challenge/the` and redirect hack's stdout to `/challenge/planet`.
I wrote `/challenge/hack 2> >(/challenge/the) > >(/challenge/planet) ` to solve the challenge and get the flag.

## CODE 
``` BASH 
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> >(/challenge/the)
You must redirect my standard output into '/challenge/planet'!
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack > >(/challenge/planet)
You must redirect my standard error into '/challenge/the'!
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> >(/challenge/the) > >(/challenge/planet)
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{ki_mPyEsAxR2DczxjGmm8MlYfRM.dFDNwYDL4YDN0czW}
``` 
## RESOURCES 
none 

