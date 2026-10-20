# Laboratory Activity 8: The Cloud Security Engineer

## Mission Overview
This laboratory activity focuses on securing a Linux server using the UFW host-based firewall. It demonstrates how to audit network access, apply a Default Deny policy, and allow only the required services.

## Objectives
- Understand the Principle of Least Privilege.
- Explain the attack surface and Default Deny policy.
- Deploy an Nginx web application using Docker.
- Configure UFW to control incoming traffic.
- Allow SSH and TCP port 8080.
- Document security configurations and maintain a GitHub portfolio.

## Commands Executed

| Command | Purpose |
|---|---|
| `docker run -d --name secure-web-app -p 8080:80 nginx` | Deploy the Nginx container |
| `curl -i http://localhost:8080/` | Test HTTP access |
| `sudo ufw allow ssh` | Allow SSH connections |
| `sudo ufw default deny incoming` | Block incoming traffic by default |
| `sudo ufw default allow outgoing` | Allow outgoing traffic |
| `sudo ufw enable` | Activate the firewall |
| `sudo ufw status verbose` | Check firewall status and policies |
| `sudo ufw allow 8080/tcp` | Allow TCP port 8080 |
| `sudo ufw status numbered` | Display numbered firewall rules |

## Skills Learned
- Linux firewall configuration
- Network port management
- Docker container deployment
- Basic server security auditing
- Applying the principle of least privilege
- Markdown documentation and GitHub portfolio management

## Screenshots
The `screenshots/` directory contains evidence of the application deployment and firewall configuration.

## Conclusion
This mission demonstrates how a host-based firewall can reduce unnecessary network exposure. Proper firewall rules, regular monitoring, and careful port management help improve server security.

