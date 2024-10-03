# More Catting Practise
## EXPLANATION 
In the third task,we have to read a file named `flag` using the `cat` command but the `flag` is in some other directory.
To solve the problem,I typed `cd /flag` in the command line which lead me to the absolute path of the `flag` file which was `/lib/python3.8/curses/flag`.
Then i typed `cat /lib/python3.8/curses/flag` in the command line where `cat` is the command and  `/lib/python3.8/curses/flag` is the argument to solve the problem.
Then i copy pasted the generated flag into the `pwn.college` site.
## CODE 
```bash
Connected!
hacker@commands~more-catting-practice:~$ cd /flag
You used 'cd'! In this level, I don't allow you to change the working directory
--- you MUST chase pass 'cat' the absolute path of where I put it on the
filesystem (which is /lib/python3.8/curses/flag).
hacker@commands~more-catting-practice:~$ cat /lib/python3.8/curses/flag
pwn.college{ENQDaSUii6p2gSnx5MWwwI6KrH6.dBjM5QDL4YDN0czW}
```
## RESOURCES 
none 
