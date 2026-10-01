# Laboratory Activity 6 — Cloud Deployment Engineer

## Mission Overview

In this mission, I worked with Docker Compose to build a small private cloud storage environment. Instead of launching each container separately, I used a YAML file to define a Nextcloud application and a MariaDB database as a connected deployment.

## Objectives

* Understand how a two-tier application is organized.
* Create a Docker Compose configuration using YAML.
* Use Nano to write a configuration file in the Linux terminal.
* Run and stop a multi-container application with Docker Compose.
* Access the Nextcloud web interface through a forwarded port.
* Apply Infrastructure as Code concepts through configuration.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

This activity helped me practice creating configuration files through the command line and managing more than one Docker container at the same time. I also learned how service names and environment variables allow containers to communicate. Most importantly, I gained experience using Docker Compose as a simple Infrastructure as Code approach for deploying a multi-container application.

