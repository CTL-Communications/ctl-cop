# Undo Changes

## Undo changes on your working directory

Undo changes to a specific file

`git restore path/to/file`

Undo change to all your files in the working directory

`git restore .`

## Undo changes on your staging directory

Undo changes to a specific file

`git restore --staged path/to/file`

Undo change to all your files in the staging directory

`git restore --staged .`

## Undo changes to files that are not currently tracked in git

Ignore changes made to an untracked file

`git clean -f path/to/file`

Ignore changes made to all untracked files and directories

`git clean -f -d`
