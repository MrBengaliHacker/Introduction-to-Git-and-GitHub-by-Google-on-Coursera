## 📝 Practice Quiz – Before Version Control

---

###  1. Your colleague sent you a patch called fix_names.patch, which fixes a config file called fix_names.conf. What command do you need to run to apply the patch to the config file?

A. diff names.conf_orig names.conf_fixed > fix_names.conf
B. diff names.conf fix_names.conf
C. patch fix_names.conf < fix_names.patch
D. patch fix_names.conf names.conf

✅ **Correct Answer:** C. `patch fix_names.conf < fix_names.patch`

### 2.You're helping a friend with a bug in a script called fix_permissions.py, which fixes the permissions of a bunch of files. To work on the file, you make a copy and call it fix_permissions_modified.py. What command do you need to run after solving the bug to send the patch to your friend?

A. patch fix_permissions.py > fix_permissions.patch
B. patch fix_permissions.py < fix_permissions_modified.py
C. diff fix_permissions.py fix_permissions.diff
D. diff fix_permissions.py fix_permissions_modified.py > fix_permissions.diff


✅ **Correct Answer:** D. `diff fix_permissions.py fix_permissions_modified.py > fix_permissions.diff`

### 3. The _____ command highlights the words that changed in a file instead of working line by line.

A. patch
B. wdiff
C. diff -u
D. diff


✅ **Correct Answer:** B. `wdiff`

### 4. How can we choose the return value our script returns when it finishes?

A. Use the patch command
B. Use meld
C. Using the exit command from the sys module
D. Use the diff command 

✅ **Correct Answer:** C. `Using the exit command from the sys module`

### 5. In addition to the original files, what else do we need before we can use the patch command?

A. Diff file
B. Version control
C. Full copy of the new files
D. exit command of the sys module

✅ **Correct Answer:** A. `Diff file`