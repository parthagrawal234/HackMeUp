# Home Sweet Home
Now it's your turn to play! In this challenge, /challenge/run will write a copy of the flag to any file you specify as an argument on the commandline, with these constraints:

Your argument must be an absolute path.
The path must be inside your home directory.
Before expansion, your argument must be three characters or less.
Again, you must specify your path as an argument to /challenge/run

## Solve
Flag - pwn.college{MOIh1rL5hw4Sc1u3tY8DHio_yEq.dNzM4QDLzQjN1czW}

```bash
hacker@paths~home-sweet-home:~$ /challenge/run ~/r
Writing the file to /home/hacker/r!
... and reading it back to you:
pwn.college{MOIh1rL5hw4Sc1u3tY8DHio_yEq.dNzM4QDLzQjN1czW}
hacker@paths~home-sweet-home:~$
```

Lesson Learned - How to use `~` in paths
