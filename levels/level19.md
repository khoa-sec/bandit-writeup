# Bandit Level 19 → 20

## Goal

Find the password.

## Solution

The password can be retrieved using the setuid program bandit20-do, which allows running commands as bandit20. Use it to execute cat and read the password file.

Command used:

ls
file bandit20-do
./bandit20-do cat /etc/bandit_pass/bandit20

## Result

Password found.
