# Module 2 – Using Git Locally

Intro to advanced Git features.
This module focuses on working with Git more efficiently on a local machine.

We will learn how to:
- Get more information from Git
- Undo and fix changes safely
- Work with branches and handle merge conflicts

---

## Skipping the Staging Area

Normally, Git follows this workflow:

modify → stage → commit


For small and simple changes, Git allows skipping the staging step.

### Commit without staging
```bash
git commit -a
```
- Automatically stages **tracked and modified files**
- Does not work for new (untracked) files
- New files still require `git add` first

### Commit with message
```bash
git commit -a -m "commit message"
```

---

## Getting More Information About Our Changes

By default, `git log` shows the commit message, author, and date.
Sometimes we also need to see **what lines actually changed**.

To view the changes included in each commit, we can use:
```bash
git log -p
```
This shows the patch for each commit, similar to `diff -u`, with `+` for added lines and `-` for removed lines.

If we want details for a specific commit only, we can use:
```bash
git show <commit-id>
```
To review changes that have not been committed yet, Git provides:
```bash
git diff
```
This shows differences between the working tree and the last commit.

To interactively review changes while staging, we can use:
```bash
git add -p
```

This lets us decide which changes should be staged and which should not.

After staging changes, we can review them using:
```bash
git diff --staged
```
All change history is stored in the repository, so Git always lets us inspect what changed, when it changed, and why.

---

## Deleting & Renaming Files

When files become obsolete or incorrectly named, Git provides commands
to remove or rename them while keeping history intact.

### Deleting files
```bash
git rm <file>
```
- Removes the file from the working tree

- Stops Git from tracking it

- Automatically stages the deletion

- Requires a commit to finalize the change

### Renaming or moving files

```bash
git mv old_name new_name
```
- Renames or moves a file

- Stages the change automatically

- Preserves file history

### Ignoring unnecessary files

Some files are automatically generated and should not be tracked.
These can be ignored using a `.gitignore` file.

- `.gitignore` itself is tracked so Git knows which files to ignore
- Helps keep `git status` output clean and relevant

`git status` is especially useful here, as it clearly shows
tracked, untracked, deleted, renamed, and ignored files.