# Extracting Specific Sections of Text
In this challenge, the /challenge/run program will give you a bunch of lines with random numbers and single characters (characters of the flag) as columns. Use cut to extract the flag characters, then pipe them to tr -d "\n" (like the previous level!) to join them together into a single line. 

```bash
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run | cut -d " " -f 2 | tr -d "\n"
pwn.college{AS4q42xXPV1184oRWsyaYsXDHax.QX3ETM3EDLzQjN1czW}hacker@data~extracting-specific-sections-of-text:~$
```
