---
layout: post
title: "MicroServices in Docker Swarm and Digital Ocean"
date: 2016-06-28
categories: microservices docker cloud
---

This post explains how to develop and deploy a solution based on **microservices in the cloud**.

The **technologies** used are the following:

- [Spring Boot](http://projects.spring.io/spring-boot/) is used to develop the microservices
  - Spring Boot Starters: Web, Session (with Redis), and Thymeleaf (UI)
- [Netflix OSS](https://netflix.github.io/) is used to orchestrate the microservices
  - Netflix Components: Eureka (auto-discovery), Ribbon (load balancing), Zuul (edge)
- [Redis](http://redis.io/) is used to persist data in memory (session)
- [Docker](https://www.docker.com/) is used to containerize microservices
  - Docker Components: Machine, Swarm (cluster), and Compose (v2)
- [DockerHub]() is used to store the Docker images
- [Digital Ocean](https://www.digitalocean.com/) is used to provision a cloud environment

The **development environment** used includes the following:

- OS: OS X 10.11.5 El Capitan
- Package Manager: [Homebrew](http://brew.sh/)
- Editor: [Sublime Text 3](https://www.sublimetext.com/3)
- Terminal: [iTerm2](https://www.iterm2.com/)
- **DevOps**: Maven 3.3, Java 1.8, Docker 1.12, Docker Machine 0.8, Docker Compose 1.8 (v2)

## MicroServices

<strong>to be completed</strong>

## DevOps

Steps are the following:

1. Clone the GitHub repository: ```git clone git@github.com:flopezlasanta/spring-web.git``` <strong>pending</strong>
2. Run ```mvn package```, to generate the fat JARs
3. Run ```sh ./cloud/digitalocean-swarm.sh```, to create the droplets and build the Swarm Cluster
{% gist 33d8c0c034f98d995e5520bbcad2990b %}
4. Run ```eval $(docker-machine env --swarm docker-swarm-manager)```, for the Swarm Docker Machine
5. Run ```docker-compose -f ./docker/docker-compose.yml up```, to launch the microservices in the Swarm
6. Run ```open http://<ip-address-swarm-manager-droplet>:8080```, to test the microservices

<strong>to be completed</strong>


