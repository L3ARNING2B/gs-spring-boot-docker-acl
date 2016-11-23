# GS SPRING BOOT APPLICATION
- using Docker & Maven
- based on Acl Strategy

< CURRENT WORK IN PROGRESS >

## RUN APPLICATION

without the Docker container
$ ./gradlew build && java -jar build/libs/gs-spring-boot-docker-0.1.0.jar

Start on localhost:8080


## BUILD DOCKER IMAGE

### Maven
$ mvn package docker:build -DpushImage
$ docker:build

### Gradle
$ ./gradlew build buildDocker

### DOCKER STOP
Stop
$ docker stop 81c723d22865

Rm
$ docker rm 81c723d22865

exemple run spring boot with gradle :
$ docker run -p 8080:8080 -t springio/gs-spring-boot-docker


##

## Source
### Spring boot
https://spring.io/guides/gs/spring-boot-docker/
https://github.com/spring-guides/gs-spring-boot-docker

### Acl strategy
https://github.com/lordlothar99/strategy-spring-security-acl