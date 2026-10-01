# Docker Compose Guide

## Overview

Docker Compose provides a way to describe multiple containers and their settings in one YAML configuration. For this deployment, the file defines a Nextcloud application and a MariaDB database that work together as one system.

## The `services:` Block

The `services:` section contains the different containers that make up the application. In this project, it includes two services: `database` for MariaDB and `app` for Nextcloud. Each service has its own image and configuration, allowing both parts of the system to be started through the same Compose file.

## Connecting Nextcloud to MariaDB

The Nextcloud container finds the database through the `MYSQL_HOST` environment variable:

```yaml
- MYSQL_HOST=database
```

The value `database` matches the service name assigned to the MariaDB container. Docker Compose provides internal networking between the services, so Nextcloud can use this service name to communicate with MariaDB without needing to enter an IP address.

## `docker run` vs. `docker-compose up -d`

The `docker run` command is normally used to create and start an individual container while specifying its settings directly in the command. In contrast, `docker-compose up -d` reads the configuration from `docker-compose.yml` and starts the services defined there together in the background.

Using Compose is useful for multi-container applications because the required configuration is kept in one file. This makes the deployment easier to repeat and reduces the need to enter many separate commands.

