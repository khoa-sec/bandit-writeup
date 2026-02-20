# Bandit Level 23 → 24

## Goal

Find the password.

## Solution

The password is retrieved by creating a script in /var/spool/bandit24/foo that will be executed by the cronjob as bandit24. The script copies the password to a readable file in /tmp.

Command used:

ls /etc/cron.d/
cat /etc/cron.d/cronjob_bandit24
cat /usr/bin/cronjob_bandit24.sh

mktemp -d

chmod +x /tmp/tmp.xxxxxxxxxx.sh
cp /tmp/tmp.xxxxxxxxxx.sh /var/spool/bandit24/foo

cat /tmp/pass24

## Result

Password found.
