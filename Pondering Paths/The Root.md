# The Root 
## EXPLANATION 
First,I connected `pwn.college` to my terminal using the SSH key.The first task was to invoke the `pwn` program using its absolute path.I solved this task by typing `/pwn` in the terminal where `/` is start of the filesystem and `pwn` is program.
`/pwn` is the absolute path.Then i copy pasted the generated flag into the `pwn.college` site.
## CODE 
```bash
adityakalra@DESKTOP-BBS45RH:~$ ssh -i./key hacker@dojo.pwn.college
Connected!
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{4rCKxIkr4Ct4T7ku3wLCaG6iAC6.dhzN5QDL4YDN0czW}
```
## RESOURCES 
none 
