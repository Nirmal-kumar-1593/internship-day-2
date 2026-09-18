# Git & Command Line Reference Guide

## 1. Essential Command Line Operations
* `pwd` - Print working directory path.
* `ls -la` - List all files, permissions, and hidden `.git` directories.
* `cd <dir>` - Change directory (`cd ..` moves one folder up).
* `mkdir <folder>` - Create a new directory.
* `touch <file>` - Create an empty file.
* `rm <file>` - Remove a file (`rm -rf <dir>` removes a directory recursively).

## 2. Git Setup & Inspection
* `git init` - Initialize a new local Git repository.
* `git clone <url>` - Download an existing remote repository.
* `git status` - Inspect tracked/untracked files and current branch state.
* `git log --oneline --graph` - View a compact visual commit history.

## 3. Staging & Committing
* `git add <file>` - Move specific file changes to the staging area.
* `git add .` - Stage all modified and untracked files.
* `git commit -m "<message>"` - Record staged changes with a descriptive message.

## 4. Branching & Merging
* `git branch` - List all local branches.
* `git checkout -b <branch-name>` - Create and switch to a new branch.
* `git checkout <branch-name>` - Switch to an existing branch.
* `git merge <branch-name>` - Combine changes from target branch into current branch.

## 5. Remote Collaboration & Synchronization
* `git remote -v` - List configured remote repositories.
* `git fetch origin` - Download remote changes without modifying local working files.
* `git pull origin <branch>` - Fetch and merge changes from the remote branch.
* `git push origin <branch>` - Upload local commits to the remote repository.

## 6. Resolving Merge Conflicts
1. Identify conflicting files via `git status`.
2. Open files in VS Code and inspect `<<<<<<<`, `=======`, and `>>>>>>>` markers.
3. Accept current, incoming, or combine both changes; delete conflict markers.
4. Stage resolved files: `git add <filename>`.
5. Complete the merge commit: `git commit -m "fix: resolve merge conflict"`.