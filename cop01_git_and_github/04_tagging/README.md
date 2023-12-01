# Tagging

## Create a tag

Create a tag on the current branch you are working on

`git tag 1.0.0-stage`

## Push a tag

Push your tag to the remote repository.
In many cases, this could trigger a deployment to a staging/production environment depending on how the deployment worfklow is setup.

`git push origin 1.0.0-stage`

## Remove a tag

If you have typed your tag incorrectly, you can delete it.

Remove a local tag

`git tag -d <tag-name>`

Remove a remote tag

`git push --delete origin <tag-name>`

