# Matching with ?
## INTRODUCTION 
In the 1st challenge, we have to learn the use of glob, specifically `?` glob.
When the command line encounters a `?` character in any argument, the shell will treat it as single-character wildcard.
This works like `*`, but only matches one character.
To solve the challenge,I had to `cd` to `/challenge` without including the `c` and `l` in the argument.So i wrote the `/challenge` as `/?ha??enge` and ran it. 
## CODE
```BASH
Connected!
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{oV2MxCahrOTjksG9DzNX_fxGXkl.dJjM4QDLxMDO1czW}
```
## RESOURCES 
none
