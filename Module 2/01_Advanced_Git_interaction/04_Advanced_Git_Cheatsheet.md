# Advanced Git Interaction – Cheatsheet

> Personal quick-reference summary of key commands and concepts from Module 2: Advanced Git Interaction.


## Committing Changes
- `git commit -a`  
  Stages and commits **tracked** files only (skips `git add`).

- `git commit -a -m "message"`  
  Quick commit with a short message.

---

## Viewing Commit History
- `git log`  
  Shows commit history (message, author, date).

- `git log -p`  
  Shows commits along with the actual code changes (patch).

- `git log --stat`  
  Shows which files changed and how many lines were added/removed.

- `git show <commit-id>`  
  Displays details and changes of a specific commit.

---

## Checking Changes
- `git diff`  
  Shows **unstaged** changes.

- `git diff --staged`  
  Shows changes that are staged but not committed.

---

## Staging Changes
- `git add <file>`  
  Stages a specific file.

- `git add -p`  
  Interactively review and stage parts of changes.

---

## File Operations
- `git rm <file>`  
  Removes a file from the repository and stages the deletion.

- `git mv old_name new_name`  
  Renames or moves a file and stages the change.

---

## Ignoring Files
- `.gitignore`  
  Specifies files or patterns Git should ignore.

- `.gitignore` itself must be tracked and committed.

---

## Useful Concept
- **HEAD**  
  Points to the currently checked-out commit (current snapshot of the project).
