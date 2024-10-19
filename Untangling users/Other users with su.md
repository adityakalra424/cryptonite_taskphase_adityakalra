# Other users with su
## INTRODUCTION
In the 2nd challenge, we have to switch to some other user ,in this case `zardus`, using `su` and then run `/challenge/run`.This can be done by passing the user you want to switch to as an argument to the `su` command.If we dont pass any arguments to `su` it will switch to `root`. To switch to the `zardus` user i wrote 
`su zardus` and then i wrote `/challenge/run` to get the flag.
## CODE
```bashConnected!
hacker@users~other-users-with-su:~$ su zardus
Password:
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{IhEWPE-RGri2BBL84lQdQnTRKnF.dZTN0UDL4YDN0czW}
```
## RESOURCES
none
