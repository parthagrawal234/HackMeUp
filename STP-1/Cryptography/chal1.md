# Challenge 1

This challenge has given challenge code and binary file

## Given Code
```python3
from itertools import cycle

flag = b"flaggg{????????????????????????????????????????}"
# len(flag) = 48
key  = b'djpakoda'
# len(key) = 8
ct = bytes(x ^ y for x, y in zip(flag, cycle(key)))

with open("ct", "wb") as ct_file:
    ct_file.write(ct)
```

This code is xor the given binary file into the key and saving it into another binary file called ct

### Solution
Ans- flaggg{w0w_g0od_j0b_V3ry_gr34t_amazing_AW35OMEE}

### Reverse Code

```python3
with open("ct", "rb") as f:
    ct = f.read()

key = b'djpakoda'
pt = bytes(x ^ y for x, y in zip(ct, cycle(key)))
print(pt)
```
