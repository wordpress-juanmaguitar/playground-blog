---
tags:
  - "on/git"
  - "on/development/local"
---

`git stash` save the changes in the working directory so they can be reapplied again (even on a different branch)

## Related commands 

- ==`git stash`== (or `git push`) save the current changes in a "pack" and a `stash@{0}`  is assigned so it can be retrieved later
	- `git stash -u`  includes untracked files
- ==`git stash apply`== re-apply the last stash saved
	- We can specify a different stash to be re-applied. Ex: `git stash apply stash@{2}`
	- To also reapply any staged files we have to do `git stash apply --index`
- ==`git stash list`==  to list all the stashes saved
- `git stash --patch`  allows you to select which changes to be included in the stash


See [Stashing and Cleaning](https://git-scm.com/book/en/v2/Git-Tools-Stashing-and-Cleaning)