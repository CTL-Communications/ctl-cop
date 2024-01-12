# build image
docker build -t linux/admin .

# run image in detached mode to ssh into the container
docker run -d -p 2222:22 --name learning-linux linux/admin

# run image in interactive mode, no need to ssh
docker run -it --rm linux/admin

# class remote repository
https://github.com/theurbanpenguin/lfcs

# Documentation for Dockerfile 
https://www.cherryservers.com/blog/ssh-into-docker-container

