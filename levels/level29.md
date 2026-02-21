# Bandit Level 29 → 30

## Goal

Find the password.

## Solution

The password is stored in a git repository, but it is hidden in another branch. Clone the repository using git clone, navigate into the repo directory, list all branches, switch to the dev branch, and check the commit changes to find the password in the README file.

Command used:

git clone ssh://bandit29-git@bandit.labs.overthewire.org:2220/home/bandit29-git/repo
cd repo
ls
cat README.md
git branch -a
git checkout remotes/origin/dev
git show

## Result

Password found.
