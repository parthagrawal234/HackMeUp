# Switching Windows (tmux)
In this challenge:

We've created a tmux session with two windows:

Window 0 has the flag!

Window 1 has your warm welcome.
### Window 1
```bash
 cat <<MSG
Welcome to the tmux window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-B 0 to switch to window 0!
MSG
hacker@terminal-multiplexing~switching-windows-tmux:~$  cat <<MSG
> Welcome to the tmux window switching challenge!
> You are currently in window 1.
> The flag is hidden in window 0.
> Use Ctrl-B 0 to switch to window 0!
> MSG
Welcome to the tmux window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-B 0 to switch to window 0!
hacker@terminal-multiplexing~switching-windows-tmux:~$
```
### Window 0
```bash
> Excellent work! You found window 0!
> Here is your flag: pwn.college{MmBn068Yu1za_10wyXVxVJMtoXm.QXwkjM4EDLzQjN1czW}> MSG
Excellent work! You found window 0!
Here is your flag: pwn.college{MmBn068Yu1za_10wyXVxVJMtoXm.QXwkjM4EDLzQjN1czW}
hacker@terminal-multiplexing~switching-windows-tmux:~$
```

I used `Ctrl-B 0` to switch to window 0 after attaching myself to screen using `tmux attach`
