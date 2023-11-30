# Add, Review and Commit Changes

This section will teach you how to review your changes before you commit them.
It will also teach you how to commit your changes.

## Add files to staging directory

Add one file

`git add path/to/file`

Add all files

`git add .`


## Review changes

See the list of files that have changed on your repository

`git status`

Review changes on your *working directory*.
Note: this will not display changes that have already been added to your staging directory.

`git diff`

Review changes to your *staging directory*.

`git diff --staged`

Note: You cannot view changes to files that have not been commited to your working or staging directory.
In other words, you cannot view changes to untracked files.

## Commit changes

This command will store changes that are currently on your *staging directory*.

`git commit –m "Your commit message"`

