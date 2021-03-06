

GIT
===


**Day 1**
---------


Introduction
------------


1. `git init` to initialize the git file.
2. `git add <file>` to add files to staging area.
3. `man git commit` or `git help commit` to search help about the commit command. You can replace the **commit** command with other commands.
4. `git status` (we all know it :P) shows the current status of the branch.
5. `git log` to get the logs of commits. Gives the hash key of the head for each commit.
6. `git log --online` to get the oneline log of commits.  Can use the has key in the **git show** command.
7. `git checkout -- <filename>` to discard file changes. Its like closing a file without saving.
8. `git commit --amend -m "<message>"` to change the previous.

Branch and Merging
------------------


1. Create a new branch using either `git branch devel` and then switch using `git checkout devel` or directly create and switch `git checkout -b devel`.
2. `git log --oneline --decorate --graph --all`  to show the commit histories over all the branches. Similarly you can use, `git show-branch --all`.
3. Merging *fast-forwards* the HEAD of master to HEAD of the branch.
4. `git log --graph --abbrev-commit --decorate` gives nice acyclic graph of commits with all the different branches.
5. The opposite of git commit -a is git add -p.

**Day2**
--------


6. `git remote -v` to see the origin.
7. `git checkout -b dev origin/dev` to switch to dev branch and start tracking the origin dev.
8. `git push -u origin cool-branch` ??
9. rebase, up stream,
10. `git diff` Shows the changes between the working directory and the index. This shows what has been changed, but is not staged for a commit.
11. `git diff --cached` Shows the changes between the index and the HEAD(which is the last commit on this branch). This shows what has been added to the index and staged for a commit.
12. `git diff HEAD` Shows all the changes between the working directory and HEAD (which includes changes in the index). This shows all the changes since the last commit, whether or not they have been staged for commit or not.


Python Gyaan
============


* Create a *.gitignore* file and add `__pycache__` and `*.pyc`. Compiled objects might create problem on other systems.
* mybinder.org, wakari.io for hosting jupyter notebooks online...
