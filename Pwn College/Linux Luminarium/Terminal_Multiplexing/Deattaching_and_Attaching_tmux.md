# Dettaching and Attaching (Tmux)
For this challenge:

Launch tmux

Detach from it.

Run /challenge/run (this will send the flag to your detached session!)

Reattach to see your prize
### Screen (tmux)
```bash
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$  echo Congratulations, here is your flag: pwn.college{wzD1lVwh9vmk24ZH5FFVnDjkJp1.QX5gjM4EDLzQjN1czW}
Congratulations, here is your flag: pwn.college{wzD1lVwh9vmk24ZH5FFVnDjkJp1.QX5gjM4EDLzQjN1czW}
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$
```
### Terminal
```bash
Connected!
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux
[detached (from session 0)]
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ /challenge/run
Found detached tmux session: 0
Sending flag to your tmux session...

Flag sent! Now reattach to your tmux session with:
  tmux attach

You'll find the flag waiting for you there!
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux a
[detached (from session 0)]
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$
```

## Solution
I used `Ctrl-B and d` to dettach from tmux and then ran /challenge/run then reattached to the session to find the flag
