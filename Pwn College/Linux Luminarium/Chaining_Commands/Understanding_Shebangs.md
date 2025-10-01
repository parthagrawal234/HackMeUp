# Understanding Shebangs
For this challenge, create a script at /home/hacker/solve.sh that has a proper shebang and outputs "hack the planet". Remember to make it executable, then run /challenge/run to verify your script works correctly!

### File script.h
```
#!/bin/bash

echo "hack the planet"
```
### Terminal
```bash
hacker@chaining~understanding-shebangs:~$ nano solve.sh
hacker@chaining~understanding-shebangs:~$ /challenge/run
Error: /home/hacker/solve.sh is not executable!
Hint: Use 'chmod' to make it executable
hacker@chaining~understanding-shebangs:~$ chmod a+x solve.sh
hacker@chaining~understanding-shebangs:~$ /challenge/run
Testing your script...
Perfect! Your flag:
Flag: pwn.college{02RI_Ifbv6tCcKFj7UUGxEI1pEY.QX5MzM4EDLzQjN1czW}

hacker@chaining~understanding-shebangs:~$
```
