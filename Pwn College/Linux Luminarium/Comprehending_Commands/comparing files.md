# Comparing Files

This challenge asks us to compare files using the diff method and find the difference between files `/challenge/decoys_only.txt` and  `/challenge/decoys_and_real.txt`

```bash
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
11a12
> pwn.college{wR0nTuphAQd8KP6owCD0RMgRRs8.QXzAzM4EDLzQjN1czW}
hacker@commands~comparing-files:~$
```

## Flag
pwn.college{wR0nTuphAQd8KP6owCD0RMgRRs8.QXzAzM4EDLzQjN1czW}

## Solution
command `diff` gives the change in the files where after 11th line of First file there is the real flag in the second file
