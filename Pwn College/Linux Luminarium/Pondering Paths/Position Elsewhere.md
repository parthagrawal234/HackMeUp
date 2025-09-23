# Position Elsewhere

This challenge will require you to execute the /challenge/run program from a specific path (which it will tell you). You'll need to cd to that directory before rerunning the challenge program. Good luck!

## Solve
Flag - pwn.college{0gQBaRsRTjDko31wYzH5qkZJEoP.ddDN1QDLzQjN1czW} 

```bash
Connected!
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/include directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /usr/include
hacker@paths~position-elsewhere:/usr/include$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{0gQBaRsRTjDko31wYzH5qkZJEoP.ddDN1QDLzQjN1czW}
hacker@paths~position-elsewhere:/usr/include$
```
