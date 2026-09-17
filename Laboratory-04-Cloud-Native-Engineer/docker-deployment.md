# Docker Deployment

## Container Lifecycle Commands

### 1. List running containers
```bash
docker ps
```
This displayed all currently running containers, showing the Nginx container
with its ID, image, uptime, and the 8080→80 port mapping.

### 2. Stop the running container
```bash
docker stop 4a69be532851
```
This gracefully shut down the running Nginx container, which stopped the web
server from responding on port 8080.

### 3. Verify it is stopped
```bash
docker ps -a
```
This listed all containers including stopped ones, confirming the Nginx
container's status had changed to "Exited."

### 4. Remove the container completely
```bash
docker rm 4a69be532851
```
This permanently deleted the stopped container and its writable layer from
the system, freeing the name and resources.
