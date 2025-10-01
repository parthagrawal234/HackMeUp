# Scripting with Arguments

For this challenge, you need to write a script at /home/hacker/solve.sh that:

Takes two arguments

Outputs them in REVERSE order (second argument first, then the first argument)

### File solve.sh
```
#!/bin/bash

echo "$2 $1"
```

### Terminal
```bash
Connected!
hacker@chaining~scripting-with-arguments:~$ nano solve.sh
hacker@chaining~scripting-with-arguments:~$ chmod a+x solve.sh
hacker@chaining~scripting-with-arguments:~$ ./solve.sh pwn college
college pwn
hacker@chaining~scripting-with-arguments:~$ /challenge/run
Correct! Your script properly reversed the arguments.
Here's your flag:
pwn.college{sHjMF8GfoUq7OAW13KfhW20GtTq.QX1MzM4EDLzQjN1czW}
hacker@chaining~scripting-with-arguments:~$
```

