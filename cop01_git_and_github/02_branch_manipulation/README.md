# Branch Manipulation

## Get latest changes to your branch

`git pull`

## Create a local branch

`git checkout -b feature/CTL-123-my-task-title`

## Track a remote branch

This is useful if you need to continue work on a branch that another developer has created already.

`git checkout --track origin/<branch-name>`

## List local and remote branches

`git branch -a`

## Switch to a different branch

`git checkout <branch-name>`

## Deleting branches

Delete a local branch

`git branch --delete <branch-name>`

Delete a remote branch

`git push origin --delete <branch-name>`

