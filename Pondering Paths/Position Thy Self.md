# Position Thy Self 
## EXPLANATION 
The third task was to navigate around directories by using the cd (change directory) command and pass a path to it as an argument.
It required me to execute the `/challenge/run` program from a specific path (which it will tell me).
So i first i executed the `/challenge/run` to find out from which directory i had to execute the `/challenge/run` program from.
The directory from which i had to execute the program from was`/usr/include`. Then i cd to `/usr/include` and reexecuted the `/challenge/run` program.Then i copy pasted the generated flag into the `pwn.college` site.
## CODE 
```bash
hacker@paths~position-thy-self:~$ cd /challlenge/run
ssh-entrypoint: cd: /challlenge/run: No such file or directory
hacker@paths~position-thy-self:~$ cd /challenge
hacker@paths~position-thy-self:/challenge$ cd/run
ssh-entrypoint: cd/run: No such file or directory
hacker@paths~position-thy-self:/challenge$ /run
ssh-entrypoint: /run: Is a directory
hacker@paths~position-thy-self:/challenge$ cd/challenge/run
ssh-entrypoint: cd/challenge/run: No such file or directory
hacker@paths~position-thy-self:/run$ cd /~
ssh-entrypoint: cd: /~: No such file or directory
hacker@paths~position-thy-self:/run$ ~
ssh-entrypoint: /home/hacker: Is a directory
hacker@paths~position-thy-self:/run$ /challenge/run
Incorrect...
You are not currently in the /usr/include directory.
Please use the cd utility to change directory appropriately.
hacker@paths~position-thy-self:/run$ cd /usr/include
hacker@paths~position-thy-self:/usr/include$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{IlGkhAntwqUYRGs6nZqVAZL_9CV.dZDN1QDL4YDN0czW}
```
## REMARK 
I didnt understand that  how do i know which directory i had to run the program from and the question said that (it will tell you) which i didnt understand at that 
moment so i had to trial and error a few times.
## RESOURCES 
none 
