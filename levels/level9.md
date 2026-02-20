# Bandit Level 9 → 10

## Goal

Find the password.

## Solution

The password is stored in the file data.txt in one of the human-readable strings, preceded by several '=' characters. Use strings to extract readable text and grep to find the line containing '=' and the password.

Command used:

ls
strings data.txt | grep =

## Result

Password found.
