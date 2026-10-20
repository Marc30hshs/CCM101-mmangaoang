

# Docker Compose Guide

## What Does the Services Block Do?

The `services:` block defines the containers required by an application. In this project, it defines two services: `database`, which runs MariaDB, and `app`, which runs Nextcloud.

## How Does Nextcloud Find the Database?

The `MYSQL_HOST` environment variable is set to `database`. Docker Compose provides service-name-based networking, so Nextcloud can use the hostname `database` to connect to the MariaDB service.

## Docker Run vs. Docker Compose Up -d

The `docker run` command is commonly used to create and start an individual container. The `docker-compose up -d` command reads a Compose configuration file and starts the defined services in the background. Compose is more convenient for applications that require multiple connected containers.

## Infrastructure as Code

Infrastructure as Code (IaC) is the practice of defining infrastructure using configuration files instead of relying entirely on manual commands. Docker Compose helps engineers deploy, manage, and reproduce application environments consistently.
