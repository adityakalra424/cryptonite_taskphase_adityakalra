# Searching For manuals
## INTRODUCTION
In the 5th challenge, we need to find the manual which will tell us how to use the `/challenge/challenge` program correctly. to do so i first i used the `man man` command to access all the command related to `man` page
.Then i found a argument `-k` which searches for text in all manual pages. Then i used it to find the text `/challenge/challenge` which helped me to find the manual for the `/challenge/challenge` which was `csjialgzrd `.
Then using that manual, i used the /challenge/challenge correctly with the correct argument with was  and then i got the flag.
## CODE
``` bash
hacker@man~searching-for-manuals:~$ man -k /challenge/challenge
csjialgzrd (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man csjialgzrd

CHALLENGE(1)                                                                                  Challenge Commands                                                                                 CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --csjial NUM
              print the flag if NUM is 905

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                                                                        May 2024                                                                                      CHALLENGE(1)
hacker@man~searching-for-manuals:~$ /challenge/challenge --csjial 905
Correct usage! Your flag: pwn.college{cE9sKV0j5_IiPalFRgJ4zrAQMTL.dZTM4QDLxMDO1czW}
```
## RESOURCES 
none
