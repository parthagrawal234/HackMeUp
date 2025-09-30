# Filtering with grep -v

This challenge asks us to grep through a standard output of a file and then search for the flag which do not contain `DECOY` to find the real flag

```bash
hacker@piping~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY
pwn.college{0cxT2FC0sL3CyQ9Xj9hDF9g-FRa.QX4ETM3EDLzQjN1czW}
hacker@piping~filtering-with-grep-v:~$
```

## Flag
pwn.college{0cxT2FC0sL3CyQ9Xj9hDF9g-FRa.QX4ETM3EDLzQjN1czW}

## Solution
I used the `grep -v` command to filter out all the flag not with the word decoy and we found the flag
