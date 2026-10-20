# Security Audit Report

## Mission Overview
This report explains essential cloud security concepts and documents the initial deployment of a web application before applying firewall protection.

## 1. Principle of Least Privilege (PoLP)
The Principle of Least Privilege means giving users and applications only the permissions they need to perform their tasks. This helps protect cloud accounts and systems from unauthorized access and reduces the damage that can happen if an account is compromised.

## 2. Attack Surface
The attack surface refers to all the possible entry points that an attacker could use to access a server or virtual machine. Open network ports, exposed applications, weak passwords, and unnecessary services can increase the attack surface.

## 3. Default Deny Policy
A Default Deny policy blocks incoming network traffic unless a specific rule allows it. This is safer because unauthorized connections are blocked automatically, reducing the need to identify and block every possible attacker individually.

## Application Deployment
An Nginx web server was deployed in a Docker container named `secure-web-app`, using port 8080 to test web access before firewall configuration.

## Evidence
- `screenshots/vulnerable-app-running.png`
