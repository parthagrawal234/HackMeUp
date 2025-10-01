# Deleting Newlines
 In this challenge, we'll inject a bunch of newlines into the flag. Delete them with tr's -d flag and the escaped newline specification!

 ```bash
Connected!
hacker@data~deleting-newlines:~$ /challenge/run | tr -d "\n"
Your line-split flag: pwn.college{Ua4013yB42tT6kumw07FE3ltX_w.QX1ETM3EDLzQjN1czW}hacker@data~deleting-newlines:~$

```
