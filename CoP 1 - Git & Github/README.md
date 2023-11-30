# Git Basics

## Basic development workflow

Clone the remote repository to your local computer. 
In order to do this, copy the git path from the repository *Code* dropdown. Make sure to select *SSH*. See image below.

![clone repo](images/cloneFromGithub.png?raw=true)

On your terminal, navigate to your repositories folder and add this repository.
The following command will automatically be set to track from your local to the remote github repository.

`git clone git@github.com:CTL-Communications/ctl-cop.git`

Create a local branch to start development work.

`git checkout -b feature/CTL-123-my-task-title`

Push your changes to the remote repository for review.

`git push`

