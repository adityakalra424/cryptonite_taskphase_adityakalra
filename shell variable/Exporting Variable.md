# Exporting Variable
## INTRODUCTION 
In the 4th challenge, we must invoke `/challenge/run` with the `PWN` variable exported and set to the value `COLLEGE`, and the `COLLEGE` variable set to the value `PWN` but not exported.To solve the challenge,I wrote
`export PWN=COLLEGE` to set the  value `COLLEGE` to the `PWN` variable and export it.Then i wrote `COLLEGE=PWN` to set the value `PWN` to the `COLLEGE` variable and then i wrote `/challnege/run` to complete the challenge.

## CODE
``` bash
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{YLalukmwAuyPvInxRv0XT200ZqS.dJjN1QDL4YDN0czW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```
## RESOURCES
none
