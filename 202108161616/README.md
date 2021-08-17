# DDAY Docker commands 

 Removing Image  `docker rmi kalilinux/kali-rolling`

**running an image `docker run -it -rm rwxrob/workspace`**

* `run` Is a pull and a start at the same time*

To see all the images in your docker 

*  `docker images`

How to see all running containers

`docker ps -a`

shows docker processes 

`--rm` removes container when you are finished using it instead of pausing

## Attach 

To get back to a paused container use the attach command 

`docker attach <name>`

Can retrieve name by using the `docker ps -a` command

***If you Type Exit while in a container it exits the container***

Restart a docker

`docker restart <name>`

**instead of docker run you can**

`docker start <name>`

`docker attach <name>`

**if you want to exit but pause press** *ctrl-pq*

see [Persistant Containers](https://github.com/Lethalz/LethalZet/tree/main/202108161940)


Stop one or more running containers
`docker stop <name>`

SEARCH ALL DOCKER REPOSITORIES

`docker search <name>`

