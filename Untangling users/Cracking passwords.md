# Cracking passwords
## INTRODUCTION
In the 3th challenge, we learn how to crack a password using `John the Ripper`.The `John the Ripper` can convert the password hash to find the real value of the password.In this challenge we have to find the password for the `zardus` user, switch to `zardus` and then run `/challenge/run` to get the flag. We are given the leak of `/ect/shadow` in the `/challenge/shadow-leak`.I wrote `john  /challenge/shadow-leak` to crack the password for `zardus` user which was `aardvark` then i switched to  `zardus` by typing `su zardus` with the password .then i wrote `/challenge/run` to get the flag.
## CODE
```bash
Connected!
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
