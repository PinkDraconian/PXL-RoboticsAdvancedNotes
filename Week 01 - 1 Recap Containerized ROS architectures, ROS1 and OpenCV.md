---
title: 'Week 01 - 1 Recap Containerized ROS architectures, ROS1 and OpenCV'
created: '2020-10-01T08:45:14.037Z'
modified: '2020-10-01T09:40:37.504Z'
---

# Week 01 - 1 Recap Containerized ROS architectures, ROS1 and OpenCV

## Difference between containers and VMs
Container provides OS-level virtualization where as a VM provides hardware-level virtualization

## Difference between containers and images
Docker images are never started or running. The `docker run` command takes the Docker image as a template and produces a container from it.

## What is Docker
Docker is a tool designed to make it easier to create, deploy and run application using containers. They allow us to package up an application with all the parts it needs, making the "it runs on my machine" obsolete

## What is a Docker registry
Application that stores and allows us to distribute Docker images

## Create Docker container from image
- `docker create <IMAGE>` (Without starting)
- `docker run <IMAGE>` (Also start container)

## What are Docker volumes
In order to save and share data between containers, volumes were created. They are directories that exists as normal directories for the host filesystem and are accessible by containers

## Create, remove and use Docker volumes
- `docker volume create <NAME>`
- `docker volume rm <NAME>`
- `docker run -v "$(pwd)":<NAME> <IMAGE>`

## List, start, attach, stop and remove Docker containers from existing Docker images
- `docker ps`
- `docker run <IMAGE>`
- `docker run -it <IMAGE> /bin/bash`
- `docker stop <CONTAINER>`
- `docker rm <CONTAINER>`

## Inspect running Docker containers
`docker inspect <CONTAINER>`

## List, remove Docker images
`docker images`
`docker rmi <IMAGES>`

## Read, write and build container images using a Dockerfile
1. Write the Dockerfile
2. `sudo docker build -t <IMAGENAME> <PATH/TO/Dockerfile>`
