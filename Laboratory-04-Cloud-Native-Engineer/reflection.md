# Reflection

## 1. How does the boot time and setup process of a Docker container compare to installing an operating system on a Virtual Machine?
The difference was dramatic. Setting up a web server on a VM means
provisioning the machine, booting a full operating system, installing the
web server package, and configuring it — easily fifteen minutes or more.
With Docker, pulling the Nginx image and running the container took only a
few seconds, because the container reuses the host's kernel and only needs
to start the Nginx process itself rather than an entire OS.

## 2. Why is port mapping (-p 8080:80) necessary when running a web server inside a container?
A container runs in its own isolated network namespace, so Nginx listening on
port 80 inside the container isn't reachable from the host by default. The
`-p 8080:80` flag creates a bridge that forwards traffic arriving at port
8080 on the host to port 80 inside the container. Without it, `curl
http://localhost:8080` would fail even though the web server is running
perfectly well inside the container.

## 3. What happens to the data inside a container when you use the docker rm command?
Removing a container deletes its writable layer, so any data written inside
the container that wasn't stored elsewhere is permanently lost. This is why
containers are described as ephemeral. To keep data beyond the container's
life, you have to use volumes or bind mounts that store the data on the host
rather than inside the container itself.

## 4. How do you think containerization changes the way software developers and IT operations teams work together (DevOps)?
Containers give both teams a single shared artifact. Developers package the
application with all its dependencies into an image, and operations runs
that exact same image in production — eliminating the environment mismatches
that used to cause friction between the two teams. This shared definition
makes automated pipelines and consistent deployments much more practical.

## 5. How is your GitHub portfolio evolving?
My portfolio now spans Linux fundamentals, infrastructure assessment,
multi-cloud comparison, and hands-on container deployment. Each lab folder
follows the same documentation structure, so it reads like a genuine
engineering portfolio rather than a set of disconnected assignments.
