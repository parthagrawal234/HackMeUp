# Moving Files

This challenge asks us to move the file `/flag` contents into the `/tmp/hack-the-planet` file

```bash
hacker@commands~moving-files:~$ mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'.
hacker@commands~moving-files:~$ /challenge/check
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{Qh0gJgUF8tQ7ryLAeCnPj5rIf7p.QX5ETM3EDLzQjN1czW}

hacker@commands~moving-files:~$
```

## Flag
pwn.college{Qh0gJgUF8tQ7ryLAeCnPj5rIf7p.QX5ETM3EDLzQjN1czW}

## Solution
I used the `mv` command to move the `/flag` to the `/tmp/hack-the-planet` and then used `/challenge/check` to get the flag
