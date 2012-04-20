shell_helpers
=============

A collection of shell helper scripts for development

squash
------

Will squash all your branch's commits into one. Usage:
    squash [branch_name]
What this script does is:

 * `Step 1` Rename target branch to a temp one
 * `Step 2` Checkout to remote master
 * `Step 3` Create a new branch out of master and checkout to it
 * `Step 4` Merge with --squash option the temp branch to the new one
 * `Step 5` Get a list of Modified and Added files by the merge
 * `Step 6` Add the Modified and Added files
 * `Step 7` Perform a commit - Editor opens
 * `Step 8` Push to origin with fast forward option (overwrite)
 * `Step 9` Delete temp branch
 