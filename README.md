# Git Hello
Hello Git

# 1. Begin

- Initializes a Git repository in current directory
- Creates a hidden folder called ".git" that contains all the necessary files and history for version control.

```bash
git init
```

- Now : the folder becomes a Git working directory, meaning you can now:
  - Track file changes
  - Use branches
  - Connect to remote repositories (e.g., GitHub)
  - Use other Git features

# 2. Connect your repo to GitHub

```bash
git remote add origin https://github.com/user/repo.git
```

# 3. Clone remote repo to PC (GitHub).

```bash
git clone https://github.com/user/repo.git
```

# 4. Stage changes 

### stage all files

```bash
git add .
```

- Add all changes in current directory & subdirectories to staging area
- that measn : “I want to include these changes in the next commit. (New, Modified & Deleted files & folders in the current directory & below
- 🛑 it's good to use a .gitignore file to exclude unwanted files.

### stage specific file

```bash
git add <file>
```

### Show changes not yet staged

```bash
git diff
```

### Show changes

```bash
git status
```
- Show me what’s going on in my working directory and staging area
- it shows:
  ✅ Which branch you’re on
  ❓ Which files have been modified
  ➕ Which files are staged (ready to commit)
  ❌ Which files are not staged yet
  🆕 Which files are untracked (new files not added to Git yet)


# 7. Commit

### commit changes with msg 

```bash
git commit -m "Message"	
```

- Create new snapshot (with unique ID) of staged changes as a commit + message describes snapshot
- ⚠️ Every time you change a file and want to commit that change, **you must "git add" it again**.

> OR :

```bash
git commit -am "Commit 2 on main"
```

- It automatically stages all changes to files that are **already tracked by Git** (were committed before) & have been modified or deleted


# 6. Branches

### List all branches

```bash
git branch
```

### Create a new branche

```bash
git branch <name>
```

### switch to existing branch
  
```bash
git checkout <name>
```

### create & switch to new branch

```bash
git checkout -b <name>
```

### Merge another branch into current one

```bash
git merge <branch>
```

### Delete a branch (after merging)

```bash
git branch -d <name>
```

# 7. Push / Pull

### Push your main branch to GitHub for the first time

```bash
git push -u origin main
```
### Get the latest changes from GitHub

```bash
git pull
```

---


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
