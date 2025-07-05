# Git Hello
Hello Git

# Setup & Configuration

git config --global user.name "Your Name"	          Set your name for Git commits

git config --global user.email "you@example.com"	  Set your email for Git commits

git init	                                          Initialize a new Git repository

git clone <url>	                                    Clone a GitHub (or other) repository to your computer

# Working with Files

git status	            Show changed files (untracked, modified, staged, etc.)

git add <file>	        Stage a specific file for commit

git add .	            Stage all changes in the current directory

git commit -m "Message"	Save (commit) your changes with a message

git rm <file>	          Delete a file and stage the deletion

git mv <old> <new>	    Rename a file and stage the change

# Branching & Merging

git branch	            List all branches

git branch <name>	      Create a new branch

git checkout <name>	    Switch to another branch

git checkout -b <name>	Create and switch to a new branch

git merge <branch>	    Merge another branch into the current one

git branch -d <name>	  Delete a branch (after merging)

# Remote & GitHub

git remote -v	                Show remote URLs (like GitHub)

git remote add origin <url>	  Connect your repo to GitHub

git push -u origin main	      Push your main branch to GitHub for the first time

git push	                    Push local commits to GitHub

git pull	                    Get the latest changes from GitHub

git fetch	                    Get changes from remote without merging

git clone <url>	              Copy a remote GitHub repo locally

# History & Logs

git log	            Show commit history

git log --oneline	  Short summary of commits

git diff	          Show changes not yet staged

git diff --staged	  Show staged changes

# Undo & Fix

git restore <file>	  Undo changes to a file

git reset <file>	    Unstage a file (but keep changes)

git reset --hard	    Undo all changes (dangerous!)

git revert <commit>	  Undo a commit by creating a new one

git stash	            Temporarily save changes without committing

git stash pop	        Reapply last stashed changes
