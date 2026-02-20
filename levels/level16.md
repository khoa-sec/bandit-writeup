# Bandit Level 16 → 17

## Goal

Find the password.

## Solution

The password can be retrieved by first scanning localhost ports from 31000 to 32000 to find the port using SSL/TLS. Then use openssl s_client to send the current password and receive the SSH private key.

Command used:

ls
nmap -p 31000-32000 --script ssl-cert localhost
cat /etc/bandit_pass/bandit16 | openssl s_client -connect localhost:31790 -quiet

## Result

Password found.
