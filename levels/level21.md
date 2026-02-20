# Bandit Level 21 → 22

## Goal

Find the password.

## Solution

The password is stored in a file created by a cronjob. Check the cronjob configuration in /etc/cron.d/, read the script it runs, and then read the temporary file containing the password.

Command used:

ls /etc/cron.d/
cat /etc/cron.d/cronjob_bandit22
cat /usr/bin/cronjob_bandit22.sh
cat /tmp/t706lds9SORqQh9aMcz6ShpAoZKF7fgv

## Result

Password found.
