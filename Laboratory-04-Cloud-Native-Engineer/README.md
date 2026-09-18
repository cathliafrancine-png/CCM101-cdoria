# Laboratory 04 – Cloud-Native Engineer

## Mission Overview

In this mission, I explored how cloud-native engineering uses containers to deploy and manage applications. I compared traditional Virtual Machines (VMs) with Containers and used KillerCoda to work with Docker. I also deployed an Nginx web server in a Docker container, verified that it was running, and managed its container lifecycle.

## Objectives

- Differentiate Virtual Machines and Containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute Docker CLI commands.
- Pull, run, manage, and terminate an Nginx container.
- Create technical Markdown documentation.
- Continue building a Cloud Computing portfolio on GitHub.

## Docker Commands Executed

### Checkpoint 3 – Verify Docker Environment

`docker --version`

`docker info`

### Checkpoint 4 – Deploy Nginx Container

`docker pull nginx`

`docker run -d -p 8080:80 --name nginx-server nginx`

`curl http://localhost:8080`

### Checkpoint 5 – Container Lifecycle

`docker ps`

`docker stop nginx-server`

`docker ps`

`docker rm nginx-server`

## Skills Learned

- Understanding the differences between Virtual Machines and Containers.
- Using Docker CLI commands in a cloud-based environment.
- Pulling and running Docker images and containers.
- Mapping host ports to container ports.
- Verifying a running web server using a local HTTP request.
- Managing the lifecycle of Docker containers.
- Creating technical documentation using Markdown and GitHub.

## Challenges Encountered

One challenge I encountered was becoming familiar with Docker commands and understanding how each command affects a container. I also needed to make sure that the Nginx container was running correctly and that port 8080 was properly mapped to port 80. Another challenge was verifying that the container was successfully stopped and removed after deployment. Through the activity, I was able to understand the Docker workflow better and document the commands and results clearly.
