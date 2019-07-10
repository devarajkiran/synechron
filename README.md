Docker:
https://www.katacoda.com/courses/docker
AWS Free Tier

## DOCKER

https://www.katacoda.com/courses/docker/deploying-first-container
$ docker version
$ docker images

## Create Docker contaniner
1. get image from https://hub.docker.com/_/hello-world
$ docker pull hello-world
$ docker run hello-world
## it will show all containers
$ docker ps -a  

## Get Tomcat Image from https://hub.docker.com/r/bitnami/tomcat
$ docker pull bitnami/tomcat
$ docker run bitnami/tomcat
## Open another terminal (+)
$ docker ps
$ docker exec 9716fb808dc5 ls bitnami/tomcat/data
$ docker stop 9716fb808dc5

## Run Tomcat image on mentioned PORT
$ docker run -P bitnami/tomcat //random port picked
$ docker run -p 8080:8080 bitnami/tomcat  // linux port: tomcat port
$ docker run -p 8091:8080 bitnami/tomcat  // linux port: tomcat port 
## View HTTP Port on 80 Terminal > Edit Port to see Tomcat Welcome page
https://2886795346-8091-cykoria01.environments.katacoda.com/sample/
