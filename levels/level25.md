# Bandit Level 25 → 26

## Goal

Find the password.

## Solution

The password is retrieved by logging in with the private key. The shell opens with more, which restricts commands. Resize the terminal to trigger more, then escape to a shell by setting /bin/bash as the shell and executing it.

Command used:

ssh bandit26@bandit.labs.overthewire.org -p 2220 -i sshkey.private

v

:set shell=/bin/bash

:shell

cat /etc/bandit_pass/bandit26

## Result

Password found.
