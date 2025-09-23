# Implicit Relative Paths, from /
Let's try it here! You'll need to run /challenge/run using a relative path while having a current working directory of /. For this level, I'll give you a hint. Your relative path starts with the letter c 😊

## Solve
Flag - pwn.college{oCvMyALlcuKUml5r3XpspmPX8e4.dlDN1QDLzQjN1czW}

```bash
Connected!
hacker@paths~implicit-relative-paths-from-:~$ challenge/run
bash: challenge/run: No such file or directory
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{oCvMyALlcuKUml5r3XpspmPX8e4.dlDN1QDLzQjN1czW}
hacker@paths~implicit-relative-paths-from-:/$
```
