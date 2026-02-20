# Bandit Level 15 → 16

## Goal

Find the password.

## Solution

The password can be retrieved by submitting the current level password to port 30001 on localhost using SSL/TLS. Use cat to read the password and pipe it into openssl s_client to send it securely.

Command used:

ls
cat /etc/bandit_pass/bandit15 | openssl s_client -connect localhost:30001 -quiet

## Result

Password found.
