---
layout: post
title: "MicroServices in Docker Swarm and Digital Ocean"
date: 2016-06-28
categories: microservices docker cloud
---

This post explains how to develop and deploy a solution based on **microservices in the cloud**.

The technologies used for this proof of concept are the following:

- [Spring Boot](http://projects.spring.io/spring-boot/) is used to develop the microservices
  - Spring Boot Starters: Web, Session (with Redis), and Thymeleaf (UI)
- [Netflix OSS](https://netflix.github.io/) is used to orchestrate the microservices
  - Netflix Components: Eureka (auto-discovery), Ribbon (load balancing), Zuul (edge)
- [Redis](http://redis.io/) is used to persist data in memory (session)
- [Docker](https://www.docker.com/) is used to containerize microservices
  - Docker Components: Machine, Swarm (cluster), and Compose (v2)
- [DockerHub]() is used to store the Docker images
- [Digital Ocean](https://www.digitalocean.com/) is used to provision a cloud environment


<strong>Note: this post will be extended with a step-by-step guide</strong>