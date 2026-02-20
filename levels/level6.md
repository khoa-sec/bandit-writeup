# Bandit Level 6 → 7

## Goal

Find the password.

## Solution

The password is stored somewhere on the server and has the following properties: owned by user bandit7, owned by group bandit6, and 33 bytes in size. Use find from the root directory with the correct options to locate the file and cat to read it.

Command used:

ls
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password

## Result

Password found.
