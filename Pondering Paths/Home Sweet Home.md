# Home Sweet Home
## EXPLANATION 
The ninth task is to run a command `/challenge/run` which will write a copy of the flag to any file i specify as an argument on the commandlinew with these contraints
1.Your argument must be an absolute path.
2.The path must be inside your home directory.
3.Before expansion, your argument must be three characters or less.
I typed `/challenge/run` as a command in the command line 
The 3rd contraint tells us that we need to use ~ in the argument to reduce the number of characters in the argument 
so i typed `~/a` as an argument which is equal to `/home/hacker/a`. This refers to the file in which the command will write a copy of the flag
Then i copy pasted the generated flag into the pwn.college site.
## CODE 
```bash
Connected!
hacker@paths~home-sweet-home:~$ /challenge/run
You must provide an argument to /challenge/run when you invoke it!
hacker@paths~home-sweet-home:~$ /challenge/run ~/adk
The argument you provided must not have been longer than 3 characters (it's
currently 5 characters long)!
hacker@paths~home-sweet-home:~$ /challenge/run ~/a
Writing the file to /home/hacker/a!
... and reading it back to you:
pwn.college{4TXeF5E4Dor3V-n_gbAX1qy3cPE.dNzM4QDL4YDN0czW}
```
## REMARK 
I didnt do this in the first try. the first try was full of nonsense command that i also dont know why i did it(trial and erroring this thing). 
After spending some time reading the previous task and their introduction i was able to understand this task and solve it.
## RESOURCES 
none 
