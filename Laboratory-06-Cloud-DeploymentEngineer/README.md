

# Mission 6: The Cloud Deployment Engineer

## Mission Overview

This laboratory activity demonstrates how to deploy a private cloud storage application using Docker Compose, Nextcloud, and MariaDB.

## Objectives

- Explain two-tier architecture.
- Create a Docker Compose YAML configuration.
- Deploy and verify multiple containers.
- Access Nextcloud using a web browser.
- Understand Infrastructure as Code.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
cat docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose logs --tail=50
docker-compose down
```

## Skills Learned

- Linux command-line operations
- YAML configuration
- Docker Compose deployment
- Multi-container networking
- Nextcloud and MariaDB integration
- Technical documentation using Markdown
