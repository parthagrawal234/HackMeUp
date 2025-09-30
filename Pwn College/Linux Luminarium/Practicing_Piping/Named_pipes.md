# Named Pipes

This challenge asks us to create a `fifo` and put the output of `/challenge/run` onto it and then cat the fifo to get the flag


### Terminal 1
```bash
palinux@LAPTOP-6CJCK5GG:~$ ssh -i key hacker@dojo.pwn.college.
Connected!
hacker@piping~named-pipes:~$ mkfifo /tmp/flag_fifo
hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo!
Bash will now try to open the FIFO for writing, to pass it as the stdout of
/challenge/run. Recall that operations on FIFOs will *block* until both the
read side and the write side is open, so /challenge/run will not actually be
launched until you start reading from the FIFO!
hacker@piping~named-pipes:~$
```

### Terminal 2
```bash
palinux@LAPTOP-6CJCK5GG:~$ ssh -i key hacker@dojo.pwn.college.
Connected!
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at
/tmp/flag_fifo! Here is your flag:
pwn.college{sRZntwrGYdAIfDsKlI2p8gNQLjr.QXzMzM4EDLzQjN1czW}
hacker@piping~named-pipes:~$
```
## Solution 
I push the output of flag into the fifo in one terminal and due to the blocking behaviour of the fifo i had to cat the fifo in another terminal to get the flag
