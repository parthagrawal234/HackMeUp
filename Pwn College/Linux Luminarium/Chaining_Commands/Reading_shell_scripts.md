# Reading Shell Scripts

In this level, we will learn to read shell scripts. /challenge/run is a shell script that requires you to put in a secret password, but that password is hardcoded into the script iself! Read the script (using, say, cat), figure out the password, and get the flag!

```bash
Connected!
hacker@chaining~reading-shell-scripts:~$ cat /challenge/run
#!/opt/pwn.college/bash

read GUESS
if [ "$GUESS" == "hack the PLANET" ]
then
        echo "CORRECT! Your flag:"
        cat /flag
else
        echo "Read the /challenge/run file to figure out the correct password!"
fi
hacker@chaining~reading-shell-scripts:~$ /challenge/run
hack the PLANET
CORRECT! Your flag:
pwn.college{owpt7s2aK9eyoDMiLP-J8hmfoRS.QXyADO4EDLzQjN1czW}
hacker@chaining~reading-shell-scripts:~$
```
This challenge i read the code of /challenge/run and when i read it i found the secret code is `hack the PLANET` i executed the file and got the flag
