# Scripting with Multiple Conditions
For this challenge, write a script at /home/hacker/solve.sh that:

Takes one argument

If the argument is "hack", output "the planet"

If the argument is "pwn", output "college"

If the argument is "learn", output "linux"

For any other input, output "unknown"
### File solve.sh
```
#!/bin/bash

if [ "$1" == "pwn" ]
then
        echo "college"
elif [ "$1" == "hack" ]
then
        echo "the planet"
elif [ "$1" == "learn" ]
then
        echo "linux"
else
        echo "unknown"
fi
```
### Terminal
```bash
Connected!
hacker@chaining~scripting-with-multiple-conditions:~$ nano solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ chmod a+x solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ ./solve.sh pwn
college
hacker@chaining~scripting-with-multiple-conditions:~$ ./solve.sh learn
linux
hacker@chaining~scripting-with-multiple-conditions:~$ ./solve.sh hack
the planet
hacker@chaining~scripting-with-multiple-conditions:~$ /challenge/run
Correct! Your script properly handles all the conditions with elif.
Here's your flag:
pwn.college{822oBngMF_pL95RmG-nqA92z9Oh.QX4MzM4EDLzQjN1czW}
hacker@chaining~scripting-with-multiple-conditions:~$
```
