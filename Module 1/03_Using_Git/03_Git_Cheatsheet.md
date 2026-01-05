# Git Cheatsheet

Quick reference of basic Git concepts and commands learned in Module 1


## Git Project Structure

Every Git project has:
- **Git directory** (`.git`) → stores history and metadata
- **Working tree** → current files you work on
- **Staging area** → changes prepared for commit

---

## Git Configuration

### Set user identity
```bash
git config --global user.email "me@example.com"
git config --global user.name "My Name"
```
Identifies who made each commit.

---

## Repository Setup

### Initialize a repository
```bash
git init
```
Creates a new empty Git repository in the current directory.

---

## File & Directory Commands

### List all files (including hidden)
```bash
ls -la
```
Used to verify the `.git` directory exists.

### View Git internal directory
```bash
ls -l .git
```
Displays the contents of the `.git` directory, which stores Git’s history, configuration, and metadata.

---

## Tracking Changes

### Stage files
```bash
git add <file>
```
Adds file changes to the staging area.

### Check repository status
```bash
git status
```
Shows untracked, modified, and staged files.

### Commit changes
```bash
git commit
git commit -m "commit message"
```
Saves staged changes as a snapshot in the repository.

---

## Commit Message Guidelines

- **Summary line:** ≤ 50 characters

- Leave **one blank line**

- **Description:** lines ≤ 72 characters

- Explain **why** the change was made

Reference: https://commit.style/

---

## Key Takeaways

- Git tracks changes using snapshots (commits)

- Staging controls what goes into a commit

- Clear commit messages improve collaboration