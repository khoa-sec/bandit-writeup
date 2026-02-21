# Bandit Level 31 → 32

## Goal

Find the password.

## Solution

The password is obtained by pushing a file to the remote git repository. After cloning the repository and reading the README file, the instructions said to create a file named key.txt with the content "May I come in?" and push it to the master branch.

However, the file was ignored due to the .gitignore file, so I forced git to add it using git add -f. Then I committed and pushed the file to the remote repository. After pushing, the server returned the password for the next level.

Command used:

git clone ssh://bandit31-git@bandit.labs.overthewire.org:2220/home/bandit31-git/repo
cd repo
ls
cat README.md
echo "May I come in?" > key.txt
git add -f key.txt
git commit -m "add key"
git push origin master

## Result

Password found.
