# Scripting with Default Cases
For this challenge, write a script at /home/hacker/solve.sh that:

Takes one argument

If the argument is "pwn", output "college"

For any other input, output "nope"
### File solve.sh
```
#!/bin/bash

if [ "$1" == "pwn" ]
then
  echo "college"
else
  echo "nope"
fi
```
### Terminal
```bash
Connected!
hacker@chaining~scripting-with-default-cases:~$ nano solve.sh
hacker@chaining~scripting-with-default-cases:~$ chmod a+x solve.sh
hacker@chaining~scripting-with-default-cases:~$ ./solve.sh pwn
college
hacker@chaining~scripting-with-default-cases:~$ ./solve.sh opp
nope
hacker@chaining~scripting-with-default-cases:~$ /challenge/run
Correct! Your script properly handles the if/else conditions.
Here's your flag:
pwn.college{4tnVQofsxo7v9lWguoVxrnTdxJU.QX3MzM4EDLzQjN1czW}
hacker@chaining~scripting-with-default-cases:~$
```
