# **Day-1**
### Basic Docker Commands and Concepts

Day one of learning **Docker 🐋** was amazing. in the session of day one i leant aboout  the basics such are how to know whether the Docker is active or inactive, and how to enable it  permanently. To know the information (like version, licence, memory, Operating System etc) of the docker use the command, ```docker info``` . Learnt about few basics like, What is Provisioning(Booting).

In any of the platform to launch or install or to start an OS we need an OS image. In Docker we need a Docker image so we can install or start an OS and in Docker world this OS is technically known as  **"Containers"**.

Learned about basic commands in Docker like: # ```docker ps: This command is used to see how many OS is running on Docker currently```.

```docker images  :  This command is used to see how many images are there.```

```docker pull <OS name>``` eg(OS name) centos:7, This command is used to download images from internet(mainly from hub.docker.com)

To launch we can use the  "docker run ```docker run <OS name>```
Learned about the command  ```docker ps -a```  which is used to know how much Docker is running.

learned about the command to add an own name:
                  ```docker run -it --name <own name> centos:7```
                    to stop the OS we can use:
                  ```docker stop <name>```

Summarising Basic Docker Commands : -
```
docker pull <os name/image name>

docker images

docker ps 

docker ps -a 

docker run <os name/image name>

docker run -it <os name/image name>

docker start <container name/ id>

docker attach <container name/ id>

docker stop <container name/ id>

docker restart <container name/ id>

ctrl + p + q --> detach from running container

docker rm <container name/ id>

docker rmi <os name/ image name>
```

### Handwritten notes are also uploaded..have a look..!
### Contributions are always welcome ❤. feel free to open full request.