# Before Version Control

## Keeping Historical Copies
Before version control systems, developers saved multiple copies of files with timestamps or version numbers, which was inefficient and error-prone.

## Diffing Files
A "diff" compares two versions of a file and shows the differences line-by-line.

## Applying Changes
You can apply differences from one file to another using tools like `patch`, which reads the output of `diff`.

## Practical Application of Diff and Patch
- `diff file1.txt file2.txt > changes.diff`
- `patch file1.txt < changes.diff`

This simulates how changes could be shared before Git existed.
