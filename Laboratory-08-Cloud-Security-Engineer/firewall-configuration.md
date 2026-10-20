# Firewall Configuration Report

## Mission Overview
This report documents the UFW firewall configuration used to secure the Ubuntu server and control incoming network traffic.

## 1. Allow SSH
```bash
sudo ufw allow ssh
```
This rule allows SSH traffic on port 22 so administrators can remotely manage the server.

## 2. Configure the Default Policies
```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```
These commands block incoming traffic by default while allowing outgoing connections.

## 3. Enable UFW
```bash
sudo ufw enable
sudo ufw status verbose
```
These commands activate the firewall and display its current status and default policies.

## 4. Allow the Web Application
```bash
sudo ufw allow 8080/tcp
sudo ufw status numbered
```
This rule allows incoming TCP traffic on port 8080 for the web application.

## 5. Verify Application Access
```bash
curl -i http://localhost:8080/
```
The curl command checks whether the Nginx application responds to an HTTP request.

## Why SSH Must Be Allowed First
If I enable UFW before allowing SSH, incoming SSH connections may be blocked and I could lose remote administrative access to the server.

## Security Best Practices
- Allow only the ports required by the application.
- Keep unnecessary services disabled.
- Review firewall rules regularly.
- Avoid exposing sensitive services to the public internet.
- Verify firewall behavior from an appropriate external test environment.

## Evidence
- `screenshots/firewall-activated.png`
- `screenshots/firewall-port-allowed.png`
