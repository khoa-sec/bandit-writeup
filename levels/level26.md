# Bandit Level 26 → 27

## Goal

Find the password.

## Solution

The password can be retrieved using the setuid program bandit27-do, which allows running commands as bandit27. Use it to execute cat and read the password file.

Command used:

ls
file bandit27-do
./bandit27-do cat /etc/bandit_pass/bandit27

## Result

Password found.
