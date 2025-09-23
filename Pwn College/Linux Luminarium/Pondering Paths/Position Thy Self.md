# Position Thy Self

This challenge will require you to execute the /challenge/run program from a specific path (which it will tell you). You'll need to cd to that directory before rerunning the challenge program. Good luck!

## Solve
Flag - pwn.college{oCJrl6KkbKMBS7D_t81sVdasgao.dZDN1QDLzQjN1czW}

```bash
Connected!
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /home directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cdhome
bash: cdhome: command not found
hacker@paths~position-thy-self:~$ cd home
bash: cd: home: No such file or directory
hacker@paths~position-thy-self:~$ cd /home
hacker@paths~position-thy-self:/home$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{oCJrl6KkbKMBS7D_t81sVdasgao.dZDN1QDLzQjN1czW}
hacker@paths~position-thy-self:/home$
```

Lesson Learned - How to change the directories and learn the cd command
