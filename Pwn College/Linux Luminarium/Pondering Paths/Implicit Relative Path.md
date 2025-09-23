# Implicit Relative Path
This challenge will need you to run it from the /challenge directory.

## Solve
Flag - pwn.college{cTCfEgx-6IehOWk5Tbp5IzaiNNl.dFTN1QDLzQjN1czW}

```bash
Connected!
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{cTCfEgx-6IehOWk5Tbp5IzaiNNl.dFTN1QDLzQjN1czW}
hacker@paths~implicit-relative-path:/challenge$
```

Lesson Learned - Naked Path in Main directory doesn't work
