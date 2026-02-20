# Bandit Level 22 → 23

## Goal

Find the password.

## Solution

The password is stored in a file created by a cronjob with a filename based on the md5 hash of "I am user bandit23". Generate the md5 hash and read the corresponding file in /tmp.

Command used:

ls /etc/cron.d/
cat /etc/cron.d/cronjob_bandit23
cat /usr/bin/cronjob_bandit23.sh
echo I am user bandit23 | md5sum
cat /tmp/8ca319486bfbbc3663ea0fbe81326349

## Result

Password found.
