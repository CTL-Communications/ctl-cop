# Welcome to your first Docker practice round!

CTL is in need of a new and flashy web app with their logo in it.
They would like to deploy this to a server somewhere so that others can view and admire the design.

Developers at CTL have been hard at work and have assembled a Nodejs web app,
particularly an Express app with handlebars view engine.

It is your job to take their great code and deploy it to a server where other users can see it.

- Short Disclaimer

We have ZERO budget for this, so the company doesn't mind if the server is up only for a short while, it's just a demo in the end :)

## Download the code

If you have `git` installed in your computer. Clone the repository to your local machine. 

`git clone https://github.com/CTL-Communications/ctl-cop`

If you already cloned this repository in the past, grab the latest updates.

```bash
git checkout main
git pull
```

## Create a DockerHub account

We are going to use a Docker lab to tinker with docker. This is provided by the Play with Docker service and it will also hold our server for free!

Login to [Play with Docker](https://labs.play-with-docker.com/)
Select a lab environment and click on `+ ADD NEW INSTANCE`

Take note of the `SSH` information provided, you will need this to transfer files from your local computer to this remote server. It should be something similart to the line below, but you will have your own ip address number and random characters after.

`ssh ip172-18-0-135-cmgkrd4nupig00ap0dug@direct.labs.play-with-docker.com`

Go back to your computer, open up a terminal and navigate to the COP repository you cloned previously.
Change directory to this first exercise folder.

`cd ctl-cop/cop02_docker/docker_example/first-container/`

Upload this directory to the instance you just created. Just replace the ssh command you where presented before with `scp -r .`

`scp -r . ip172-18-0-xxx-xxxxxxxxxxxxxxxx@direct.labs.play-with-docker.com:/root`

Let's build and run our CTL application!

```bash
docker build -t ctl .
docker run -d --name ctlsite -p 8080:8080 ctl
```

Did it succeed?

Click on `OPEN PORT` button at the top of the page, type in `80` and amaze yourself with the magic design!

