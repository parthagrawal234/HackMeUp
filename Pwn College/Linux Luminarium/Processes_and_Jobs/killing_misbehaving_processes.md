# Killing Misbehaving Processes

In this challenge, there's a decoy process that's hogging a critical resource - a named pipe (FIFO) at /tmp/flag_fifo into which (like in the Practicing Piping FIFO challenge) /challenge/run wants to write your flag. You need to kill this process.

### Terminal 1
```bash
Connected!
hacker@processes~killing-misbehaving-processes:~$ ps -ef | grep /challenge/decoy
root         139       1  0 07:05 ?        00:00:00 su -c exec /challenge/decoy > /tmp/flag_fifo hacker
hacker       142     139  0 07:05 ?        00:00:00 /usr/bin/python /challenge/decoy
hacker       213     183  0 07:06 pts/1    00:00:00 grep --color=auto /challenge/decoy
hacker@processes~killing-misbehaving-processes:~$ kill 142
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
hacker@processes~killing-misbehaving-processes:~$
```

### Terminal 2
```bash
palinux@LAPTOP-6CJCK5GG:~$ ssh -i key hacker@dojo.pwn.college.
Connected!
hacker@processes~killing-misbehaving-processes:~$ cat /tmp/flag_fifo
pwn.college{VDqp8JJfNK1xSkia2o7Q5QfyguV-T3Rc1Q.1PFWCBYxoSW}
pwn.college{oT-rUsMJcHnTnTTNbSLJClXPwW9A8VpoGqVj2iDgLji5oz}
pwn.college{zrr29K7bluLBHT0cNSmKMOPRjriFrkvt1Cc5OnKxJL8X4B}
pwn.college{9s765LgQtnGhTKx7TJxr8aFMfAx80jfVA4EHuM56udnsHb}
pwn.college{5mrtqhx.khZcZYm6rZGelYLtZNo765IxEj6OvS.v27ZrKI}
pwn.college{.GTUCphTCrpeHCRhoGc7-vLzyIWWi0MU28J72qObK6e7Jl}
pwn.college{-uhbXnumZe3vc96keVihPVQPBedaoRXIsl-FeBUGTCbBFy}
pwn.college{bKMg3V4e1c2g.pJ3Lv.2Cl43Hg.AwCHo2SpwlzLTM0cbB5}
pwn.college{Wf561myKmhi4G7e0UT1wQzvpE8UQ7KAfxjb3fbSPZihTSW}
pwn.college{gsCiVn9PFWsjDvA1P2YoTxFeJEk.Xj.q633uf0gN37s57X}
pwn.college{1sRmPlMDx3zKsV4HLzOkjQxVJwIuLUFe2F9npjQpGp5tlP}
pwn.college{xv0sVqbR4ZYyqcF4-F-LhqYaaRhIcgYoZ1HUY4ntweEb3w}
pwn.college{PWtaZ3xiJ8C3.X7SnxWriQwq.ErNGC-d-3oZf6M.zyWWbO}
pwn.college{6JcOBg4kV80BhHLtEZDhgOR4h5MeSUGUuJ24XkFhUITiv-}
pwn.college{vC3uUX2hnOdRp.qMvkmpseImEIdJdJ1paKTmGE3LK9x6je}
pwn.college{jGaBu40MGRXDsy1lH1.L.dJJM-lLykV.4zBaf9DqmSbrUW}
pwn.college{coUpKdEEu10pMofJmFhKhhDHslrb5lCg0zvugMGoooe.qE}
pwn.college{6IpO6uhqiD-CpPvpfQIHsfVDYXflmJzDvHzLsp5jdcmSqy}
pwn.college{PiwPJu.ckaha1kxr3AeyBzf9hBl109bJOd7d.PGko2MjOg}
pwn.college{9PNlQyvgln2Wfyw99-HYhqUZf-VqfpnG4r75aWg-mpxG3d}
pwn.college{uRok1A7kvYKtxvcWMnGWF-HxhUjem0fHkogh-K8IgWQs0N}
pwn.college{ERjEDivqqiq39WDtWJRb61i2VTjQQo3vuISIC1w-MJccYl}
pwn.college{RcJYMwTED0whIWMKKM7UBur5Kc6JGtlmBqTazDAcmx.Ex2}
pwn.college{3ujJb5CtYXe9VkbExlDP1Dy6n7xGK9foFjES24.SsIwQoz}
pwn.college{zyhSutercvEuWXFWTgP9eNkoq8L92uDTpF9CUyk0qYdhsn}
pwn.college{YcD82qGnl6mV5uLj39ZeLjlzt7Tihbc4zuC7KiW2npI379}
pwn.college{aooat3s.TYpXbpE3TMDA28YJ.tCIP-1P2hS3muZhjZbJyp}
pwn.college{Kk9nDX617GybGCf75n52YXnVv70yF9hdlRegNC0kHYHoTO}
pwn.college{HFf54XR9tScbWHYmB.n1zM2GwuTb87bjpfSeh--dCT426F}
pwn.college{MVBm1eAiCFFzScSzofoya9y7VV3BQs-FQNionFMu8TJ.dm}
pwn.college{JbPSohjLXc7BERujoAxW3IkxK870CdbzqLjgpO583lBFYl}
pwn.college{Abn37FOjCKi.o2rPpbtcnheZc237gB4T5K9I5OvuEgq3cV}
pwn.college{jOPMqyLXYPMgKRsE174VwhGs-8i1npYpc2SRX7mAz0J2cc}
pwn.college{jtCnrKVi1i52g1gLqOvVe1TLzM94LMx4C5TC5lYjmztBOu}
pwn.college{Oe6Ue-9LMUmWVwP1gfdYj1nClIf1eEhL7GbK3O4jN890F4}
pwn.college{7kKCFC.fuHCuuhpbk2AgW3Hyk1RY-LTWOz-Du0vcyreB9Z}
pwn.college{PSrYhfCzfdmMlFar0aGwRoGasVjtHOXPjYxv1qQp.2fDho}
pwn.college{C2JRkytI1exb1FRUkyHY6w2HEYpw0aHHogSlySM5GZn4qt}
pwn.college{xzVN9dWEux19meeW40MPixYD2sgQ0cJnrG.HPgxDCtJF2H}
pwn.college{hwm3TtsTLmBOupm4Dgtq2kHMj6m7RW4Qbz17NgxcDuYpG0}
pwn.college{Z2RDF9EZjzhHUohSVZBfJ38b2DgkG9.kkdN9ojx.4KqR0c}
pwn.college{duJm-75JnvOFfYYv2LxthC8bOS6S3s-iY0qVQTV5b9LV4U}
pwn.college{Htna8faVHgeCMslVRmFIqX9I2KpC3t13BUyV5x-BUPFrkX}
pwn.college{B1bGBtcfIxZHkR3jZhFYApsEPq6UDIrA1lOUIznKSg6rFT}
pwn.college{umdj5RRRUoHeChoL8YfAQ5TFIEbHiN4fjHMLqkq4uNMAjM}
pwn.college{xYLXIDakGuGCLOCKkn4HHf7IjOZMcpNS0-XZeK7xrUdRwZ}
pwn.college{ehR6XJA0FfOcisPDSmlwgkNGZz3hEyiSh7UFZ3OP6clXhT}
pwn.college{oDkRld8YZC6W9fvZ00P53J1WAxa.V-TMMd8MNoqEk99o4m}
pwn.college{8KjaVQpUEs76XnlMRq4Dv5PczeSGY-hnoHzGkwoV3ldMd6}
pwn.college{0KzVEceFDosP-bHqHjPLhkXp8o8F7jwIFXHHnS12-WZ2lR}
pwn.college{YrcGa-kgBn8YFm6eGDupbOQwHqa2ZBBFNvSZ7oWsNpY1X4}
pwn.college{P.RA0uMNFV.NOWIG7QF445zPnLJUfuW8yCpd5iRhJ6mj92}
pwn.college{r4Te33S45RLH7ZPq0aBdZF56lyIxKf0NGNDOyPJ0IW.0Nv}
pwn.college{CJ-KEfWGYbVns0xLR280g8J6Y-t62OnJipUP2Lix1c1mJH}
pwn.college{DepW3Qowta1Jy0KRYbCxWIo4hCw4RSFhhifuniSuFuiHFk}
pwn.college{9Zd8jmcEZaOPagfXJ2Tmb3X1vDHH2VNk84q6u.iut00aZ5}
pwn.college{uNk5EGNtOqvJiaQP-kl6qzb5Nfri83dqwZopyOSsXW-mNz}
pwn.college{ksI8ktA5sRC9i4Npo4ajrBjxmOO5iStS7UB6Z9A9uKcOuj}
pwn.college{7.HHEnVc0LuMoaGiFcI7NSa7kVM6bC22pKT4omROIDHBKp}
pwn.college{bRPkKbQ60WohHXoeCndiB5ISiTS69xG52Za-SGZx4pTxm-}
pwn.college{qi-pcBcBwL1aXcde1OVg3IWnxmQZmcWRp.zu3iWLl9pV-D}
pwn.college{di-WDYNehkjNOEqutK0YbTRSDVbVOT6D.bqQTS7lmQIfiF}
pwn.college{0FjU-wCPer1XZFCHKK74qXdLIHp81aGcKafUGqq6aMLbjs}
pwn.college{ihmNnMgf87HsD5AhMV7oRAHEp2cJ1EXjHi1NX5o44dMKEL}
pwn.college{fjlgnoi5-KoSco9yVzd0mNZFLmN--suac2Ce3nFCvLTJdR}
pwn.college{dWf3dy6qg5.NbUhYkTfNX4zxK17h31J6EHcAyWaj.DMjTT}
pwn.college{d1Fn6u6Tje1DCjiS6QS5SMJjvsxnIvQ8R6NjTne--J8VGK}
pwn.college{KkAI30PYBuj28bnkpXSJcNInxE3.yf7BTPM4ygrO32AcRA}
pwn.college{980U-iFBimFnrXQQlFHNhc2IDibOQ4xX4-m7ogL2h-OiBa}
pwn.college{86KyPO2a7f.FZhkvXiIEzy0ke-e7.eVyQFS5kP-kbXIMu5}
pwn.college{5od0imhkmvjkshR.KiOnMKy9KcIE-gOjj4iH823odeIY5K}
pwn.college{F8LaNuab9EaOAIYDXxn0diJG462DA-8-vj17zPyOtPduBI}
pwn.college{2o4gnax6sOyuE6C8VgZG5pjXtgDd9Nax-AE4PuKqU07T39}
pwn.college{3LiBFR1uL9FY5Fm08iC.m2ytvLvD2Ft9iygvHcBM02jzMq}
pwn.college{gCQVnmrHvheGxU.Rw.z783hzzchMwdGjdY.ev4aExGNv84}
pwn.college{J2kGlPg5ZbfhxbSUUB9bBFj8ir7hP7lEyNSpzvWgLHdTME}
pwn.college{2S1DyJ8ht2dsPMA1R8Rg8nGER4wXNzzJzjRl3xeGnAu6Hh}
pwn.college{VYHZecorZD8j7kynv2GcvYKjdXtlPrhDgtAMbG8flw7g3Y}
pwn.college{5eySlAi7C-MRrwqX8aZ6Ged.CoWZUUWmvzNQtfCQzqkUtC}
pwn.college{JI-wN9ksXV9XvGhWrOSkuDoEKzBJjkANlRACEbhXYg8h0G}
pwn.college{PYy50AIAUIjimbAc.THvSdtzCeiuFt0S00o1Fl7vWe8gA-}
pwn.college{0rhyk08NgI00cMuX0Idx94Jpnx742wdzb0mKrnIQkyr9L1}
pwn.college{d-bjhmLpy5KztyQodBK1rgfpxv0WS2FotifJ6MxXIvRwxP}
pwn.college{Q-qnt-F0.4LTRQxEt9qWuhEhMdp3U9hMlgl7I1oMV4nZ44}
pwn.college{s4Y8sASwS00yT.kfbq8Mtj1gjWf11pmVijt2uv69NR3Gai}
pwn.college{qc7Ed6Us4SOhTztPvjO.yNgrzCqbBWMWnNr2p3a16sfNET}
pwn.college{nYww3jGEACdhzjDFaCtDRJt1QgoZ1ywqKVIkHOOA.p2Rqw}
pwn.college{qUmScsqY5TcMEIM-TvblXS8oOOghvQoW7xwl.leHiqdBZQ}
pwn.college{KNd90viJX76v0oM0YUsjMwVswu.Uhri2vrv8B2k0ACUPyT}
pwn.college{fK05Vcz.Vr-Wflpnc5defgYQuQf9XppAcIva4OQ.-QG3EY}
pwn.college{Q9f1Ph.tsHlXbWewGXN1UQ31ALO7ZojIiNqr5EdtBQcTte}
pwn.college{hCMDERAbiqfylNkG79UP2QktcBUlLs056fn8.zCA.V0gZz}
pwn.college{l6TGU2oWr95P1HMLUDzIpsT9C8j8hyHEG8eHaguQbTQiie}
pwn.college{YT805fa5Glh.6RzV5-egdRPTcdluXsjsRY.Fcn5Ji-e3tB}
pwn.college{whTMoCJHruYgsCCt1ocPxoJIpcOdo0Mq3KbNV7Edz9QeoG}
pwn.college{KWKqiq0lWt0KhTQcjHLXSEAlNfIKo1YoSfyqLqVV9G5XUU}
pwn.college{ECw-f4YwcRls.gx4eFRZEbW0pOEHER4TmUUuNHF2EFonWM}
pwn.college{-DJyU7LDKq7KzrJRNspSdEs1BThgDofHO4knUFz6fB7zcI}
pwn.college{yr5Il3msb2Bjxpgu6a8Z5s22Sto5Be2SEmJ0tUpL7FrN3K}
pwn.college{IGO9D2xiLiMNuwFRh5NIHii8rd10vJp-TBn1LjQrVwAmhd}
pwn.college{bf4B7Ia9.DMbOpbmir4pxWyNtY2zMS5ovfo-HAWVBI8sVi}
pwn.college{dAwe2njVRbyB-Nt5zhRjp9kYm50XOzeAksaxhVgVkbRZru}
pwn.college{weqwzXqDuADu-mE-Kr7BtNIdDUtOsot0w-Uk9kpZp7jCZV}
pwn.college{uyGPZSE4qYFt6R62HnPhX6Bz2x8hW6mB-A3ejwuiJ2CtE9}
pwn.college{ojohr4W8Ir1HV8kEWfQmU6JosoA9Qzo6v-LKYTRNaRjpm0}
pwn.college{WBgbV8hpv2qYGPHNIRlzVmnprKTm7MEAW9Y4uIyvg9EQR5}
pwn.college{lBQXcDh5dy03hE.jt9hnxs4YiLr2O.Su-Kh5TCENkIWsag}
pwn.college{wnqg.XtlqbkWDBVpeBtLEU4XBjFGCFz5Rid.lbKMGwXzp4}
pwn.college{WjbA.uFcO0kX9iM2D5kjMpy.FFNtf-PtKhcuGX8mQfK6Bq}
pwn.college{POIG56prJuhrfAq9Psb3SlUhUWQSgitHS9PIJhJ47js2BT}
pwn.college{8MtonWDqYJ8wO1Bol1sK9gsbLVoVUcwNBFQDqumotdz5RR}
pwn.college{YI4rLIaOTFWO3HL7Ug-F-EA8C869jrqkExw4YN8HOg64UP}
pwn.college{4DQqOybrxqK0mmtwQ4ctgOXrq5BBl5vd8oOFivNlds5xt9}
pwn.college{I46VIWc4uf5Q5zo5iuiHKbGpfn6SVuk03afbMhMxk4zFqt}
pwn.college{w4NWXjC7pSDMfH2zEUOGJDG0x1k7wxgN-2NHQ8VmcSMT3K}
pwn.college{JOCgbLff7tx15mPcPaETAaicKdp6onPGouIeKwxfNe02rh}
pwn.college{3Gi7GkMVyiCnvR7CZgdXzdv9fCIw0VkKl-4uKDq9OTUrhz}
pwn.college{.xjLrlFfx5qQMhAnymd-RsEkRBrwbCjKc5Fnbhr.QqxvHz}
pwn.college{xF.M.YfiVCjVkq906s8YausbXVQm9GexxRwbF9OlaEliDg}
pwn.college{y2WloYscgNOnkAuoysTC1rgY1YmOv6Ptg210G.I30Spirq}
pwn.college{LsunNSU2GD3PrRBkY0k4UDVRY9qwOCdfhvbBiWN1JP9jFG}
pwn.college{I1bjQCnKL0cdSK1shFa4bhlY3Fvdb-izBi1KD4SnXtY7A.}
pwn.college{EdyykvsVaL54lINYgKmjJS5EWXywRxGoq3qToNmrXM5Xsn}
pwn.college{Wz4E4r-bSCka2XGXy4xvOaw7BKMc6lEQJXdnKidbNqcQCX}
pwn.college{jg4sU1xgSK9sezZIQLBQFPBygEueA6aQfDTMvL1SCMEUjt}
pwn.college{7h4XfoAP6GLlst8Bgl7uAxZlEfRVtzBJxCmc0Q8T22Lic4}
pwn.college{q-oUmfwFgplVKSzV6jep.6rv-XrYm3f1EoFUD3HRS83CHU}
pwn.college{xA7PXs5AQyyvVA3yGdYBaxMuTRf5Zks5huwy9QKC5rurMM}
pwn.college{-tQfqbG7uHetqiZEQOPGzm.8wfvhfGPMWbcQ-Bc-l3ie90}
pwn.college{n4st1F0u-DM69HvFBOtmnruD7J4uja364FWFQOt48Uzgeb}
pwn.college{YCi2WYXJHpYZu58U9I1SLJ9WidRsJwecaKFzRzht-leL1D}
pwn.college{PXtRtlmOjSmbPG3CFA.4pnmR.RrkvvZF-50rdz6a1eo3s7}
pwn.college{WHKKZfftnML684uxU.XuM-CqmgR4htInatL4m3u8u9pRCj}
pwn.college{g8yCYnOBRic4m6PMn2OmQiUFL-wkOF7UM9x3LrO5myHeZv}
pwn.college{eAyZxcSgRLxvmI7Eh-YUD8IqtUbVpNUUd6aGERC52QaId7}
pwn.college{0nISZx4L8EzESqUIKq62UUkadI5JUoybPWwujMfR-4E8zo}
pwn.college{I5OhQXodW7laR675v0e3-ElPxSz.QX0MzM4EDLzQjN1czW}
pwn.college{I5OhQXodW7laR675v0e3-ElPxSz.QX0MzM4EDLzQjN1czW}
^C
hacker@processes~killing-misbehaving-processes:~$ cat /tmp/flag_fifo
pwn.college{I5OhQXodW7laR675v0e3-ElPxSz.QX0MzM4EDLzQjN1czW}
```

## Solution
This challenge has some issues i see a process /challenge/decoy sending decoy flags to the /tmp/flag_fifo fifo file and this makes problem for me to get the flag from /challenge/run so i kill see the process and it is with PID 142 i kill it then run /challenge/run which prints the flag on fifo but the old buffer also comes through so i run it again and cat in another flag to get the flag
