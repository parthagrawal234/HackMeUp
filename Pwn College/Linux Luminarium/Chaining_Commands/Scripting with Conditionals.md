# Scripting with Conditionals

For this challenge, write a script at /home/hacker/solve.sh that:

Takes one argument

If the argument is "pwn", output "college"

For any other input, output nothing
### File solve.sh
```
#!/bin/bash

if [ "$1" == "pwn" ]
then
  echo "college"
fi
```
### Terminal
```bash
Connected!
hacker@chaining~scripting-with-conditionals:~$ nano solve.sh
hacker@chaining~scripting-with-conditionals:~$ chmod a+x solve.sh
hacker@chaining~scripting-with-conditionals:~$ ./solve.sh pwn
./solve.sh: line 3: [pwn: command not found
hacker@chaining~scripting-with-conditionals:~$ nano solve.sh
hacker@chaining~scripting-with-conditionals:~$ ./solve.sh pwn
college
hacker@chaining~scripting-with-conditionals:~$ ./solve.sh own
hacker@chaining~scripting-with-conditionals:~$ /challenge/run
Correct! Your script properly handles all the conditions.
Here's your flag:
pwn.college{swztGU50LeTammPZ1yD9BdvI1TJ.QX2MzM4EDLzQjN1czW}
hacker@chaining~scripting-with-conditionals:~$
```
