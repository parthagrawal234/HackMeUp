# Finding Session


### Screen 1
```bash
hacker@terminal-multiplexing~finding-sessions:~$  echo 'Wrong session! Keep looking.'
Wrong session! Keep looking.
hacker@terminal-multiplexing~finding-sessions:~$
```
### Screen 2
```bash
hacker@terminal-multiplexing~finding-sessions:~$  echo 'Wrong session! Keep looking.'
Wrong session! Keep looking.
hacker@terminal-multiplexing~finding-sessions:~$
```
### Screen 3
```bash
hacker@terminal-multiplexing~finding-sessions:~$  echo 'Congratulations! You found the right session!'
Congratulations! You found the right session!
hacker@terminal-multiplexing~finding-sessions:~$  echo pwn.college{wioepdBQ5W0sl3xxNvYZkGSolnI.QX3gjM4EDLzQjN1czW}
pwn.college{wioepdBQ5W0sl3xxNvYZkGSolnI.QX3gjM4EDLzQjN1czW}
hacker@terminal-multiplexing~finding-sessions:~$
```
### Terminal
```bash
Connected!
hacker@terminal-multiplexing~finding-sessions:~$ screen -ls
There are screens on:
        193.pts-0.terminal-multiplexing~detaching-and-attaching (Remote or dead)
        207.pts-1.terminal-multiplexing~detaching-and-attaching (Remote or dead)
        144.session_d13b77cda3ddd348    (Detached)
        147.session_bc9c206f94979a5e    (Detached)
        150.session_8e3ef217c4d21551    (Detached)
5 Sockets in /home/hacker/.screen.
hacker@terminal-multiplexing~finding-sessions:~$ screen -r session_d13b77cda3ddd348
[screen is terminating]
hacker@terminal-multiplexing~finding-sessions:~$ screen -r session_bc9c206f94979a5e
[detached from 147.session_bc9c206f94979a5e]
hacker@terminal-multiplexing~finding-sessions:~$ screen -r session_8e3ef217c4d21551
[detached from 150.session_8e3ef217c4d21551]
hacker@terminal-multiplexing~finding-sessions:~$
```
