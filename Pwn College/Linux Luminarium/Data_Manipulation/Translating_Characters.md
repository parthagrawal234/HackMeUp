# Translating Characters
In this level, /challenge/run will print the flag but will swap the casing of all characters (e.g., A will become a and vice-versa). Can you undo it
 
```bash
Connected!
hacker@data~translating-characters:~$ /challenge/run | tr ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ
yOUR CASE-SWAPPED FLAG:
pwn.college{4JOQkPRLrCj-kyML_VGtCc2oKpr.QXzETM3EDLzQjN1czW}

hacker@data~translating-characters:~$
```

## Solution

I used the `tr` command to change the all uppercase to lowercase and lowercase to uppercase to find the flag
