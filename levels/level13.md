# Bandit Level 13 → 14

## Goal

Find the password.

## Solution

The password is stored in the SSH private key. Save the private key to a file and use ssh with the -i option to log in to the next level.

Command used:

echo "PRIVATE KEY" > sshkey.private
ssh bandit14@bandit.labs.overthewire.org -p 2220 -i sshkey.private

## Result

Password found.
