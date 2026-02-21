# Bandit Level 30 → 31

## Goal

Find the password.

## Solution

The password is stored in a git repository, but it is not in the README file or commits. After cloning the repository and checking the README file, nothing useful was found. By listing the tags using git tag, I found a tag called secret. Showing the content of this tag using git show secret revealed the password.

Command used:

git clone ssh://bandit30-git@bandit.labs.overthewire.org:2220/home/bandit30-git/repo
cd repo
ls
cat README.md
git show
git tag
git show secret

## Result

Password found.
