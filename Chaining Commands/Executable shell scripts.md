# Executable shell scripts
## INTRODUCTION 
In the 4th challenge,we have to make a shellscript that will invoke `/challenge/solve`, make it executable, and run it without explicitly invoking `bash`.I wrote 
`nano file.sh` to create a shell script names `file.sh`then i wrote the command `/challenge/solve` in the file and saved it and exited from the text editor. Then i made it executable by using the `chmod` command as i wrote `chmod u+x file.sh` in the terminal.Then i wrote `./file.sh` to run the file without the use of `bash`.Then i got the flag.
## CODE
```BASH 
Connected!                                                                        
hacker@chaining~executable-shell-scripts:~$ nano file.sh
hacker@chaining~executable-shell-scripts:~$ ls -s file.sh
4 file.sh
hacker@chaining~executable-shell-scripts:~$ chmod u+x file.sh
hacker@chaining~executable-shell-scripts:~$ ./file.sh
Congratulations on your shell script execution! Your flag:
pwn.college{IPL6AZoELTZvma4R-_Ns1Bu7uUL.dRzNyUDL4YDN0czW}
```
## RESOURCES
none
## REMARK
i didnt include the lines from the text editor 

