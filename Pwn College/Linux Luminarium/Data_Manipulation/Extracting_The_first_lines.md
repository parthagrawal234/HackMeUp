# Extracting the First Lines with head
This challenge's /challenge/pwn outputs a bunch of data, and you'll need to pipe it through head to grab just the first 7 lines and then pipe them onwards to /challenge/college, which will give you the flag if you do this right! Your solution will be a long composite command with two pipes connecting three commands

```bash
Connected!
hacker@data~extracting-the-first-lines-with-head:~$ /challenge/pwn | head -n 7 | /challenge/college
Congratulations, you piped the right codes!
pwn.college{w9AZTtckT6xgSqc9be5ywhCQxKk.QX2ETM3EDLzQjN1czW}
hacker@data~extracting-the-first-lines-with-head:~$
```
