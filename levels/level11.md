# Bandit Level 11 → 12

## Goal

Find the password.

## Solution

The password is stored in the file data.txt and is encoded using ROT13. Use tr to decode the text by rotating the letters and display the password.

Command used:

ls
cat data.txt
cat data.txt | tr "A-Za-z" "N-ZA-Mn-za-m"

## Result

Password found.
