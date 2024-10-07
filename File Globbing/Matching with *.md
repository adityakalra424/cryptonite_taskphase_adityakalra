# Matching with *
## INTRODUCTION 
In the 1st challenge, we have to learn the use of glob, specifically `*` glob.When the command line encounters a `*` character in any argument,
the shell will treat it as "wildcard" and try to replace that argument with any files that match the pattern.To solve the challenge,I had to `cd` to `/challenge` without the argument being more than 4 character.
So i wrote `/challenge` as `/ch*` which is 4 characters and passed it as an argument.
## CODE
```bash
Connected!
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /challenge
You specified the path to 'cd' to in more than 4 characters. Disallowed!
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /ch*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{AKUKMIlrNMNxGotmZ8_KXPFRLZS.dFjM4QDLxMDO1czW}
```

## RESOURCES 
none
