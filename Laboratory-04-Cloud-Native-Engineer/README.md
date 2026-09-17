# Laboratory Activity 4 – Mission 4: The Cloud-Native Engineer

## Mission Overview
This activity covers the shift from traditional virtualization to
containerization. Acting as a Cloud-Native Engineer for a client complaining
about slow, RAM-heavy Virtual Machines, I researched the architectural
differences between VMs and containers, then deployed a live containerized
Nginx web server using Docker on KillerCoda and documented every command so
the client's IT team can replicate it.

## Objectives
- Differentiate between traditional Virtual Machines (VMs) and Containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute fundamental Docker CLI commands.
- Pull, run, manage, and terminate a containerized application (Nginx).
- Create professional technical documentation of container operations using Markdown.
- Continue developing a well-organized GitHub Cloud Computing Portfolio.

## Docker Commands Executed
| Command | Purpose |
|---|---|
| `docker --version` | Verify Docker is installed and check its version |
| `docker info` | Check the current status of the Docker environment |
| `docker pull nginx` | Download the official Nginx image from Docker Hub |
| `docker run -d -p 8080:80 --name my-nginx nginx` | Run Nginx in detached mode, mapping host port 8080 to container port 80 |
| `curl http://localhost:8080` | Verify the web server is responding |
| `docker ps` | List currently running containers |
| `docker stop my-nginx` | Stop the running container |
| `docker ps -a` | Verify the container is stopped (shows all containers) |
| `docker rm my-nginx` | Remove the container completely |

## Skills Learned
Explaining the architectural differences between VMs and containers;
verifying a Docker installation; pulling images from Docker Hub; running a
container in detached mode with port mapping; managing the full container
lifecycle (run, list, stop, remove); and documenting technical procedures
clearly enough for another team to reproduce.

## Challenges Encountered
Understanding port mapping was the trickiest part — grasping that the
container has its own isolated network and that `-p 8080:80` is what bridges
the host to the container took some thinking. It was also surprising how
fast a containerized web server starts compared to provisioning a VM, which
made the resource-efficiency argument much more concrete.
