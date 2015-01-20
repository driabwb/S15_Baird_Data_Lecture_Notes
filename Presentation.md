# Git Version Control System

## Topics
* What is git?
* Workflow
* Initilization
  * `init`
  * `clone`
* `branch`
* `checkout`
* `add`
* `commit`
* `merge`
* `pull`
* `push`
* `status`
* Topics of further interest
  * `log`
  * `remote`
  * `stash`
  * *.gitignore*

## Workflow

### Workflow in a picture:

|Untracked|Unmodified|Modified|Staged|*Remote*|
|---------|----------|--------|------|--------|
|These are not yet in the repo|These have not changed since the Head|These have changed since the head|These are waiting to be commited|Files in at a remote repo's head|
|`add` or *.gitignore*||`add`|`commit`|`pull`, `push`|

1. File starts untracked
  * git understands that the file is there
  * git will not do anything about the file being there
2. File is unmodified
  * git will watch for the file to change
3. File is modified
  * git sees the file has changed and awaits it being staged
  
### A basic workflow:
1. Initialize the repository
2. Add existing items to the repository: `git add`
3. Commit the existing items to the repo with an appropriate: `git commit`
4. Create a new branch
5. Checkout the new branch
6. Modify contents of the branch
7. Merge branch back into master
8. Repeat from step 4

### A basic workflow with a remote repository:

1. Clone the previously existing repo
2. Create a new branch
3. Checkout the new branch
4. Modify the contents of the branch
5. Checkout the master branch
6. Pull from the remote repo(s)
7. Merge from your branch to the master branch
8. Pull from the remote repo(s)
9. Push to the remote repo(s)
10. Repeat from step 2


## Initialization
The beginnings of the repository.

### `init`
Usage: `git init`

Does the background work to start a git repository in the current directory which has no files currently tracked.

### `clone`
Usage: git clone *remote_repository_address*

Creates a new git repository in the current directory that is a copy of the remote repository given.

**This will create another directory below your current directory for the repository.**

## Branching

### `branch`
Usage:
1. git branch
  * review the branches in the repository
2. git branch *new_branch_name*
  * create a new branch
3. git branch -d *new_branch_name*
  * delete the branch

**Note:** Creating a branch does not change your current branch.

### `checkout`
Usage:
1. git checkout *branch_name*
  * Change to the branch
2. git checkout *commit*
  * Move the current state of your copy to a particular commit

## `add` and `commit`

### `add`
Usage: git add *file* ...
* Add stage one or more files

### `commit`
Usage: git commit -m "Commit Message"
* The -m flag is optional: without it the result drops you into the default editor to create the message

## Merging

### `merge`
Usage:
1. git merge *branch_name*
  * Merges the named branch into the **current** branch

### How to Resolve Conflicts
1. Open a file with a conflict
2. Find the conflict
  * Conflicts are begun with <<<<<<< yours:name_of_file
  * Differences are seperated by =======
  * Conflicts end with >>>>>>> theirs:name_of_file
3. Remove the markers and choose the lines of code which should not be in the result of the merge.
4. Save the file.
5. Repeat from 1 until there are not more conflicts.
6. Add and commit the results of the merge.

## Pull and Push

### `pull`
Usage: git pull [remote_repository] [branch_name]
* The two parameters are optional if the defaults are set.

### `push`
Usage: git push [remote_repository]
* This pushes all the updated branches to their equivalent in the remote repository.

## Status

This gives the status of files in the repository.

Whether they are:
* untracked
* unmodified
* modified, but changes are not staged
* staged

## Topics of further interest
* `log`
  * gives a history of commits
  * particularly useful for finding the hash to checkout a particular commit
* `remote`
  * setup remote knowledge of remote repositories
* `stash`
  * Similar to the concept of shelving in other VCS
* *.gitignore*
  * Allows git to ignore untracked files without marking them as untracked.
 
