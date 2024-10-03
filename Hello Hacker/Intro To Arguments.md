# Intro To Arguments
## EXPLANATION 
First,I connected `pwn.college` to my terminal using the SSH key. Then i solved the second task which was to run the `hello` command with the argument as `hackers`.
I typed hello hackers in the terminal where `hello` is the command and `hackers` is the argument.Then i copy pasted the generated flag into the `pwn.college` site.
## CODE 
```bash
adityakalra@DESKTOP-BBS45RH:~$ ssh -i ./key hacker@dojo.pwn.college
Connected!
hacker@hello~intro-to-arguments:~$ hello hackers
Success! Here is your flag:
pwn.college{Q9UPLh2WbfIBsBKnYxqWuL5gDpV.dhjNyUDL4YDN0czW}
```
## RESOURCES 
none 
