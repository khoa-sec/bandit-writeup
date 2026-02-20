# Bandit Level 20 → 21

## Goal

Find the password.

## Solution

The password can be retrieved by using the suconnect program, which connects to a port and sends the password if the correct current password is received. First, use nc to listen on a port, then run suconnect and provide the port number.

Command used:

ls
nc -lvp 55555
./suconnect 55555

## Result

Password found.
