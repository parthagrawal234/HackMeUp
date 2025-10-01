# Finding Commands
In this challenge, we added a win command somewhere in your $PATH, but it won't give you the flag. Instead, it's in the same directory as a flag file that we made readable by you! You must find win (with the which command), and cat the flag out of that directory!In this challenge, we added a win command somewhere in your $PATH, but it won't give you the flag. Instead, it's in the same directory as a flag file that we made readable by you! You must find win (with the which command), and cat the flag out of that directory!

```bash
Connected!
hacker@path~finding-commands:~$ which win
/challenge/paths/28777/win
hacker@path~finding-commands:~$ cat /challenge/paths/28777/flag
pwn.college{0L7M-_PvZUe9tgvYz5mnU3PSM2V.QX3MTM3EDLzQjN1czW}
hacker@path~finding-commands:~$
```

I found the right directory which has the win command and then cat the flag from the same directory to find the flag
