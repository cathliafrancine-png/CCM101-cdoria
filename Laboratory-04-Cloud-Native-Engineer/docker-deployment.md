# Docker Deployment
## Container Lifecycle

1. `docker ps` → This command lists all containers that are currently running.
2. `docker stop nginx-server` This command stops the running Nginx container named nginx-server.
3. `docker ps` → This command verifies that the Nginx container is no longer running.
4. `docker rm nginx-server` → This command completely removes the stopped nginx-server container.
