# Reading Manual
## INTRODUCTION 
In the 3rd challenge, we have to read the manual page for challenge and find out how to use `/challenge/challenge` correctly. We can open the manual page using the `man` command.

## CODE
```bash
Connected!
hacker@man~reading-manuals:~$ man challenge

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

       --oaqhji NUM
              print the flag if NUM is 016

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                                                                        May 2024                                                                                      CHALLENGE(1)
hacker@man~reading-manuals:~$ /challenge/challenge --oaghji 016
Incorrect usage! Please read the challenge man page!
hacker@man~reading-manuals:~$ /challenge/challenge --oaqhji 016
Correct usage! Your flag: pwn.college{oUQaYKqhj0ih1G6IbpzAnxdAXcN.dRTM4QDLxMDO1czW}
```
## RESOURCES
none
