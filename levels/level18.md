# Bandit Level 18 → 19

## Goal

Find the password.

## Solution

The password is stored in the readme file in the home directory. Since normal login is not allowed, use ssh with the command option to directly execute cat readme and display the password.

Command used:

ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme

## Result

Password found.
