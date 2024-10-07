# Matching with []
## INTRODUCTION 
In the 3rd challenge, we learn `[]`.The square brackes are, essentially, a limited form of `?`, in that instead of matching any character,
`[]` is a wildcard for some subset of potential characters, specified within the brackets.
To solve the challenge we have to run `/challenge/run` with a single argument that bracket-globs into `file_b, file_a, file_s, and file_h`.It can be done using `[]` and writing the argument as `file_[bash]`.
## CODE 
```bash
Connected!
hacker@globbing~matching-with-:~$ cd /challenge/files
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[bash]
You got it! Here is your flag!
pwn.college{waq5zq2Onog-C6Ce7nxC3-thL1o.dNjM4QDLxMDO1czW}
```
## RESOURCES
none
