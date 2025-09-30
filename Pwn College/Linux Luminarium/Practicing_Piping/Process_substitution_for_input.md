# Process Substitution for Input

This challenge asks us to compare the output of two commands `/challenge/print_decoys` and `/challenge/print_decoys_and_flag` to find the flag

```bash
hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
83a84
> pwn.college{kBiJUtG4mJeJ2LGcVlwMR8PIycu.QX2AzM4EDLzQjN1czW}
hacker@piping~process-substitution-for-input:~$
```

## Flag
pwn.college{kBiJUtG4mJeJ2LGcVlwMR8PIycu.QX2AzM4EDLzQjN1czW}

## Solution
I used `<(command)` to make temporary files of the `/challenge/print_decoys` and `/challenge/print_decoys_and_flag` and gave them to the diff command to compare
