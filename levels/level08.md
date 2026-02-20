# Bandit Level 8 → 9

## Goal

Find the password.

## Solution

The password is stored in the file data.txt and is the only line that occurs once. Use sort to sort the file and uniq -u to find the unique line, then display the password.

Command used:

ls
sort data.txt | uniq -u

## Result

Password found.
