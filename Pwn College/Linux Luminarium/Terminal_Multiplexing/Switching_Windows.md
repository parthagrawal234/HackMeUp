# Switching Windows
For this challenge, we've set up a screen session with two windows:

Window 0 has... well, you'll have to switch there to find out!
Window 1 has a welcome message

### Window 1
```bash
Welcome to the window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-A 0 to switch to window 0!
MSG
hacker@terminal-multiplexing~switching-windows:~$  cat <<MSG
> Welcome to the window switching challenge!
> You are currently in window 1.
> The flag is hidden in window 0.
> Use Ctrl-A 0 to switch to window 0!
> MSG
Welcome to the window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-A 0 to switch to window 0!
hacker@terminal-multiplexing~switching-windows:~$
```
### Window 0
```bash
hacker@terminal-multiplexing~switching-windows:~$  cat <<MSG
> Excellent work! You found window 0!
> Here is your flag: pwn.college{kJ5BR-EBLkAqXKEAwuqal0Zy6iF.QX4gjM4EDLzQjN1czW}> MSG
Excellent work! You found window 0!
Here is your flag: pwn.college{kJ5BR-EBLkAqXKEAwuqal0Zy6iF.QX4gjM4EDLzQjN1czW}
hacker@terminal-multiplexing~switching-windows:~$
```

### Terminal
Connected!
hacker@terminal-multiplexing~switching-windows:~$ screen -r
[screen is terminating]
hacker@terminal-multiplexing~switching-windows:~$
```
