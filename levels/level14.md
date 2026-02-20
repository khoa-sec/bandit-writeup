# Bandit Level 14 → 15

## Goal

Find the password.

## Solution

The password can be retrieved by submitting the current level password to port 30000 on localhost. Use cat to read the password and pipe it into nc to send it to the port.

Command used:

ls
cat /etc/bandit_pass/bandit14 | nc localhost 30000

## Result

Password found.
