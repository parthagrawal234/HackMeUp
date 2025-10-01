# Launching Screen
For this challenge, we've hooked things up so that just launching screen will get you the flag.

```bash
palinux@LAPTOP-6CJCK5GG:~$ ssh -i key hacker@dojo.pwn.college.
Connected!
hacker@terminal-multiplexing~launching-screen:~$ screen
Congratulations! You're inside a screen session!
Here's your flag:
pwn.college{cGT3biQ_y4X3ONUrn0FCvRPsgWJ.QX1gjM4EDLzQjN1czW}
[screen is terminating]
hacker@terminal-multiplexing~launching-screen:~$
```

## Solution
When i launch a screen it gives me some rules and then the flag
