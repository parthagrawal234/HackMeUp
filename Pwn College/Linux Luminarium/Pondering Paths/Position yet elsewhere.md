# Position Yet Elsewhere
This challenge will require you to execute the /challenge/run program from a specific path (which it will tell you). You'll need to cd to that directory before rerunning the challenge program. Good luck!

## Solve
Flag - pwn.college{wXRDNm5YDchCKNiZtuNzPEMICSL.dhDN1QDLzQjN1czW}

```bash
Connected!
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /tmp directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /tmp
hacker@paths~position-yet-elsewhere:/tmp$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{wXRDNm5YDchCKNiZtuNzPEMICSL.dhDN1QDLzQjN1czW}
hacker@paths~position-yet-elsewhere:/tmp$
```
