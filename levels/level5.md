# Bandit Level 5 → 6

## Goal

Find the password.

## Solution

The password is stored in a file somewhere under the inhere directory and has the following properties: human-readable, 1033 bytes in size, and not executable. Use find with the correct options to locate the file and cat to read it.

Command used:

cd inhere
ls
find . -type f -readable -size 1033c ! -executable 2>/dev/null
cat ./maybehere07/.file2

## Result

Password found.
