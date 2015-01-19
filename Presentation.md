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
* *.gitignore*
* `status`
* Topics of further interest
  * `log`
  * `remote`
  * `stash`

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
1. Initialize the repository (repo)
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
