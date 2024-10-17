# 
## INTRODUCTION
In the 8th challenge, we had to add the `SUID bit` to the `/challenge/getroot` program in order to spawn a `root shell` for you to cat the flag ourself.
The `Set User ID" (SUID)` permissions bit allows the user to run a program as the owner of that program's file.
we can excute the `SUID bit` using `chmod  u+s`.So i typed `chmod u+s /challenge/getroot` to add the `SUID bit` to the `/challenge/getroot` program.Then i wrote
`/challenge/getroot` to make me the `root` user and then i wrote `cat /flag` to get the flag.
## CODE
```bash
Connected!
hacker@permissions~the-suid-bit:~$ ls -l
total 48
-rw-r--r-- 1 hacker hacker    4 Oct  8 19:21 COLLEGE
drwxr-xr-x 2 hacker hacker 4096 Oct  8 19:37 Desktop
-rw-r--r-- 1 hacker hacker    8 Oct  9 11:15 PWN
-rw-r--r-- 1 root   hacker   58 Oct  3 16:43 a
-rw-r--r-- 1 root   hacker    0 Oct  4 21:01 cmd1_output
-rw-r--r-- 1 hacker hacker  194 Oct  7 04:16 college
-rw-r--r-- 1 root   hacker   77 Oct  9 12:43 file
-rw-r--r-- 1 hacker hacker  829 Oct  9 10:55 instructions
-rw-r--r-- 1 root   hacker   77 Oct  6 18:15 intercepted_data
-rw-r--r-- 1 root   hacker   77 Oct  9 12:41 intercepted_data.txt
drwx------ 2 root   root   4096 Oct 11 22:31 lost+found
-rw-r--r-- 1 hacker hacker   93 Oct  9 10:55 myflag
lrwxrwxrwx 1 hacker hacker    5 Oct  4 16:19 not-the-flag -> /flag
-rw-r--r-- 1 hacker hacker    0 Oct  9 12:39 output_flag
-rw-r--r-- 1 hacker hacker    0 Oct  4 20:56 pwn
-rw-r--r-- 1 root   hacker    0 Oct  9 12:34 reason
-rw-r--r-- 1 hacker hacker  435 Oct  8 19:42 the-flag
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{4k9Ji3md3BK5OrtBWsm4zxZ6dzl.dNTM2QDL4YDN0czW}
root@permissions~the-suid-bit:~#
```
## RESOURCES
none
