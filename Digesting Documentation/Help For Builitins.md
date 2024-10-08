# Help for builitins
## INTRODUCTION
In the 7th challenge we have to learn the use of `bultins` specifically `help`.we will use `help` to lookup its instructions which will help to figure out the secret value to pass to the `bultin challenge`. And get the flag.
## CODE 
``` BASH
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "EzfCEUvo".
hacker@man~help-for-builtins:~$ challenge --secret EzfCEUvo
Correct! Here is your flag!
pwn.college{EzfCEUvodFiobTmDM6RinZ8jygB.dRTM5QDLxMDO1czW}
```
## RESOURCES 
none 
