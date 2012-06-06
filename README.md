shell_helpers
=============

A collection of shell helper scripts for development

squash
------

Will squash all your branch's commits into one. Usage:

    squash [branch_name] [optionally set a checkout source e.g. upstream/next]

What this script does is:
 * `Step 1` Rename target branch to a temp one
 * `Step 2` Checkout a fresh copy from remote master to a new branch
 * `Step 3` Merge with --squash option the temp branch to the new one
 * `Step 4` Get a list of Modified and Added files by the merge
 * `Step 5` Add the Modified and Added files
 * `Step 6` Perform a commit - Editor opens
 * `Step 7` [Prompt to] Push to origin with fast forward option (overwrite)
 * `Step 8` [Prompt to] Delete temp branch
 

searchReplace
------------
Very plain one liner search & replace. Usage: 

    searchReplace [file pattern] [regexp search] [regexp replace]

But really, just copy paste it on your shell...