 ## what is Docker? 
 
 A Docker is a set of platform service products that use OS-level virtualization to deliver software in packages called containers. The great advantage of Docker is that it makes your deployment easy and when the time comes you can even deploy it on multiple machines with almost no extra effort.



## Basic Terminologies

1- Docker Image — In very simple terms docker image is just like an ISO image file used to install any OS. You can view all docker images(publicly available on DockerHub)

2- Docker Container — When a Docker Image runs it becomes a Docker Container. You can run the same image again and a different docker container will be created.

3- Dockerfile — A Dockerfile contains all the code to set up a docker container from downloading the docker image to setting the environment.


### Docker File
ockerfiles are instructions. They contains all of the commands used to build an image.

#### Know the Commands  
FROM:Required on top of the file. Initializes a new build stage and sets the Base Image

RUN: Will execute any commands in a new layer, Can use multible times.

CMD: Provides a default for an executing container. There can only be one CMD instruction in a Dockerfile

LABEL: Adds metadata to an image

EXPOSE: Informs Docker that the container listens on the specified network ports at runtime

ENV: Sets the environment variable <key> to the value <value>
 
ADD: Copies new files, directories or remote file URLs from <src> and adds them to the filesystem of the image at the path <dest>.
 
COPY: Copies new files or directories from <src> and adds them to the filesystem of the container at the path <dest>.
 
ENTRYPOINT: Allows for configuring a container that will run as an executable

VOLUME: Creates a mount point with the specified name and marks it as holding externally mounted volumes from native host or other containers

USER: Sets the user name (or UID) and optionally the user group (or GID) to use when running the image and for any RUN, CMD, and ENTRYPOINT instructions that follow it in the Dockerfile

WORKDIR: Sets the working directory for any RUN, CMD, ENTRYPOINT, COPY, and ADD instructions that follow it in the Dockerfile

ARG: Defines a variable that users can pass at build-time to the builder with the docker build command, using the --build-arg <varname>=<value> flag
 
ONBUILD: Adds a trigger instruction to the image that will be executed at a later time, when the image is used as the base for another build

HEALTHCHECK: Tells Docker how to test a container to check that it is still working

SHELL: Allows the default shell used for the shell form of commands to be overridden



## Sources
https://gist.github.com/sd031/13699e946213c773b9246f8274794229

https://towardsdatascience.com/docker-made-easy-for-data-scientists-b32efbc23165

