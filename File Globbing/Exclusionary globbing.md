# Exclusionary globbing
## INTRODUCTION 
In the 6th challenge,we learn about glob inverts `!` or (in newer versions of bash) a `^` that bracket instance matches characters that aren't listed.
To solve the challenge we have to `cd` to `/challenge/files` and run `/challenge/run` with all files that don't start with `p, w, or n`
we can do this by running the argument as `[!pwn]*`, `[!pwn]` implies that the start can't be the letters `p, w, or n` and why only the starting letter, that is taken care of my the `*` glob.
## CODE
```bash
Connected!
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{QBN1sUGjYMr6lRNZeWhj5p0N07k.dZjM4QDLxMDO1czW}
```
## RESOURCES
none


