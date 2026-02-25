# Git Commands Reference

A quick reference for the most common Git commands used when working on this portfolio project.

---

## Setup

```bash
# Configure your name and email (only needs to be done once)
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

---

## Starting a Repository

```bash
# Initialize a new Git repository in the current folder
git init

# Clone an existing repository
git clone https://github.com/dlkilfaba-cmyk/My-Portfolio.git
```

---

## Checking Status

```bash
# See which files have changed or are staged
git status

# See a compact version of the status
git status -s
```

---

## Staging Changes

```bash
# Stage a specific file
git add index.html

# Stage all changed files at once
git add .

# Stage specific file types
git add *.css
```

---

## Committing Changes

```bash
# Commit staged changes with a message
git commit -m "Your commit message here"

# Stage all tracked files and commit in one step
git commit -am "Your commit message here"
```

---

## Pushing Changes

```bash
# Push to the default remote (origin) on the current branch
git push

# Push to a specific remote and branch
git push origin main

# Push and set the upstream branch (first push of a new branch)
git push -u origin main

# Push all branches
git push --all origin

# Force push (use with caution — overwrites remote history)
git push --force origin main
```

---

## Pulling Changes

```bash
# Pull the latest changes from the remote
git pull

# Pull from a specific remote and branch
git pull origin main
```

---

## Branching

```bash
# List all local branches
git branch

# Create a new branch
git branch feature/my-new-feature

# Switch to a branch
git checkout feature/my-new-feature

# Create and switch to a new branch in one step
git checkout -b feature/my-new-feature

# Delete a branch (after merging)
git branch -d feature/my-new-feature
```

---

## Merging

```bash
# Merge a branch into the current branch
git merge feature/my-new-feature
```

---

## Viewing History

```bash
# Show the commit log
git log

# Show a compact one-line commit log
git log --oneline

# Show changes in the last commit
git show
```

---

## Undoing Changes

```bash
# Discard changes in a file (restore to last commit)
git checkout -- index.html

# Unstage a file (keep changes, just un-stage)
git reset HEAD index.html

# Undo the last commit but keep changes staged
git reset --soft HEAD~1

# Undo the last commit and discard changes
git reset --hard HEAD~1
```

---

## Typical Workflow for This Project

```bash
# 1. Check what has changed
git status

# 2. Stage your changes
git add .

# 3. Commit with a descriptive message
git commit -m "Update hero section copy"

# 4. Push to GitHub
git push origin main
```
