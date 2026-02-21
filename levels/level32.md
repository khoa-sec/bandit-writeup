# Bandit Level 32 → 33

## Goal

Find the password.

## Solution

After logging into bandit32, I was placed in an uppercase shell that converts all commands to uppercase. Normal commands like ls do not work properly.

To bypass this restriction, I used $0 which starts a new shell. This gave me a normal shell environment. Then I listed the files and found the password file in /etc/bandit_pass/bandit33 and read it using cat.

Command used:

$0
ls
cat /etc/bandit_pass/bandit33

## Result

Password found.
