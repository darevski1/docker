## Docker Essentials

Basic docker cheat cheets

To install container run from  terminal

    sudo docker run hello-world

To check the status of all running Docker containers, you can use the command:

    docker ps

To check the status of all Docker images that are currently on your system, you can use the command:

    docker images

To check the status of all Docker containers, including those that are not currently running, you can use the command:

    docker ps -a

To check the status of a specific Docker container, you can use the command:

    docker container inspect <container_id>

To check the status of the Docker daemon itself, you can use the command:

    systemctl status docker

Search for images 

    docker search OR docker search image_name

example

    docker search ubuntu

To pull the image you can run

    docker pull name_of_the_image

Create conatiner from the image we pull

    docker run name_of_the_image

Make container to run and connect od container

    docker run -it name_of_the_container /bin/bash

To keep container run in background

    docker run -it -d name_of_container

The docker attach command allows you to attach your terminal to the container's console, so you can interact with it as if you were running commands directly on the container.

    docker attach container_name_or_id

The docker restart --unless-stopped command is used to restart a Docker container that has stopped or exited, and also ensures that the container is restarted automatically if the Docker daemon is restarted or if the system is rebooted.

    docker -it -d -p 8080:80 restart --unless-stopped container_name




