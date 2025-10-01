# Detaching and Attaching
For this challenge, you'll need to:

Launch screen

Detach from it.

Run /challenge/run (this will secretly send the flag to your detached session!)

Reattach to see your prize
### Screen
```bash
hacker@terminal-multiplexing~detaching-and-attaching:~$
hacker@terminal-multiplexing~detaching-and-attaching:~$ echo Yes! Flag is: pwn.college{sETXxvAMY8Xzw1td1K7Lzn2wGfo.QX2gjM4EDLzQjN1czW}
Yes! Flag is: pwn.college{sETXxvAMY8Xzw1td1K7Lzn2wGfo.QX2gjM4EDLzQjN1czW}
hacker@terminal-multiplexing~detaching-and-attaching:~$
```
### Terminal
```bash
Connected!
hacker@terminal-multiplexing~detaching-and-attaching:~$ screen
[detached from 173.pts-1.terminal-multiplexing~detaching-and-attaching]
hacker@terminal-multiplexing~detaching-and-attaching:~$ /challenge/run
Found detached screen session: 173.pts-1.terminal-multiplexing~detaching-and-attaching
Sending flag to your screen session...

Flag sent! Now reattach to your screen session with:

  screen -r

You'll find the flag waiting for you there!
hacker@terminal-multiplexing~detaching-and-attaching:~$ screen -r
Remove dead screens with 'screen -wipe'.
[screen is terminating]
hacker@terminal-multiplexing~detaching-and-attaching:~$
```
