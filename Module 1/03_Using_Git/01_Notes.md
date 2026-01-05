### Using Git

## First Steps with Git
Before using Git, basic configuration is required to identify who made each change. This is done using `git config` to set the user name and email. A Git repository can be created using `git init` or copied from an existing repository using `git clone`.

When a repository is initialized, Git creates a hidden `.git` directory that stores the project history and metadata. The files outside this directory form the working tree, where changes are made. Files must be added to the staging area using `git add` before they can be saved. Changes are permanently recorded using `git commit`, which stores them in the repository history.

---

## Tracking Files
A Git project consists of three main areas: the **Git directory**, the **working tree**, and the **staging area**. The Git directory stores the history of the project as snapshots created by commits. The working tree contains the
current version of the files, and the staging area holds changes that are ready to be committed.

Files in Git can be tracked or untracked. Tracked files move through three states: **modified**, **staged**, and **committed**. Modified files have changes that are not yet saved. Staged files have been marked to be included in the next commit. Committed files are stored safely in the Git history as snapshots.

---

## The Basic Git Workflow
The typical Git workflow follows a simple cycle. First, a repository is created using `git init`, which sets up the Git directory. Files are then created or modified in the working tree. New or modified files must be added to the staging area using `git add`.

Once the desired changes are staged, they are permanently saved by running `git commit`. Each commit creates a snapshot of the project and records a commit message describing the change. Only staged changes are included in a commit, while untracked or unstaged files are ignored. This cycle of modify, stage, and commit forms the core Git workflow.

---

## Anatomy of a Commit Message
A good commit message explains what changed and why it was changed. It helps future readers understand the purpose of a commit.

The first line is a short summary (about 50 characters), followed by a blank line. The remaining lines describe details of the change, with each line kept under 72 characters for readability.

Clear commit messages avoid vague words and make project history easier to understand using `git log`.
