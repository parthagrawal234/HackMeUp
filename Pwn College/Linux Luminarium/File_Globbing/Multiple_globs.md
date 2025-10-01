# Multiple Globs
This challenge asks us to run the /challenge/run command from /challenge/files directory and find files there that contain p and give it to /challenge/run

```bash
hacker@globbing~multiple-globs:~$ cd /challenge/files
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{g-HRQMtWiWOjTKvXtXYb_J3Uv6Y.QXycTO2EDLzQjN1czW}
hacker@globbing~multiple-globs:/challenge/files$
```

### Solution
I went to the /challenge/files and use `*p*` to search for any files containg p and gave it to /challenge/run to get the flag
