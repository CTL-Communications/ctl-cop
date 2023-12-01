# Basic development workflow

## Clone remote repository

Clone the remote repository to your local computer. 
In order to do this, copy the git path from the repository *Code* dropdown. Make sure to select *SSH*. See image below.

![clone repo](../images/cloneFromGithub.png?raw=true)

On your terminal, navigate to your repositories folder and add this repository.
The following command will automatically be set to track from your local to the remote github repository.

`git clone git@github.com:CTL-Communications/ctl-cop.git`

## Create a local development branch

First, make sure to pull the latest changes! you want to start with the most updated version of the code

`git pull`

Create a local branch to start development work on your assigned task.

`git checkout -b feature/CTL-123-my-task-title`

## Add and submit your changes

Add changes you have made to the *staging directory*

`git add path/to/file`

Commit your changes to the repository

`git commit –m "Your commit message"`

Push your changes to the remote repository

`git push`

Note: If you haven't setup your branch to track on remote, git will prompt you with a message to set upstream tracking.
Just copy the code and execute it in your terminal

`git push --set-upstream origin feature/CTL-123-my-task-title`

## Create a Pull Request to review your code

On Github, create a Pull Request to review your code before commiting to the *main* or *develop* branch.

![create pr](../images/createPR.png?raw=true)

Please make sure that your *base branch* is correct, if you are meant to merge your changes against *develop* change your base branch to point to *develop*.
Locate your feature branch and then click on *Create Pull Request*.

![create pr](../images/createPR2.png?raw=true)

Sometimes, Github will automatically pick up that you are intending to create a new PR and display a message to create a PR on the main screen.

![create pr](../images/createPR3.png?raw=true)

Your Pull Request should now appear on the *Pull Request* list.

![create pr](../images/createPR4.png?raw=true)

Click on the PR title, this will take you to the main pull request page.
Copy the link of the main PR page and send it to another developer for review.

