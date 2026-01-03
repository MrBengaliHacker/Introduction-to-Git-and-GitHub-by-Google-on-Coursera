# Before Version Control

## Introduction
In IT, scripts and configuration files change over time as systems grow and requirements evolve. Managing these changes requires clear historical records of what was modified and when. Version control systems provide documentation, support rollbacks, and reduce human error. They help teams maintain a healthy codebase and collaborate safely on shared projects. This module introduces version control and the tools used before Git.

---

## Keeping Historical Copies
Before version control, people kept multiple copies of files to return to earlier versions and track changes. This approach was manual and inefficient, making it difficult to know who changed what and why. It is considered a primitive form of version control.

---

## Diffing Files
Comparing files manually by looking at them side by side is error-prone. The `diff` command provides an automatic way to compare two files or directories and show only the lines that changed.

### Diff
The `diff` tool shows the differences between files. In the basic output, lines marked with `<` indicate removed lines, and lines marked with `>` indicate added lines.

Using the `-u` option displays changes with surrounding context, which makes the updates easier to understand.

---

## Applying Changes
Instead of explaining code changes manually, developers can share a diff file that clearly shows what was modified.

### Patch
While `diff` generates the differences between files, the `patch` command applies those differences to the original file automatically.

---

## Practical Application of Diff and Patch
```bash
diff file1.txt file2.txt > changes.diff
patch file1.txt < changes.diff
```