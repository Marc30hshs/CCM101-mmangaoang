

# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is an application design that separates the web application and the database into two different layers. These layers communicate with each other to provide services to users.

## The Web/Application Tier

The web/application tier uses Nextcloud to provide the user interface. It handles HTTP requests and allows users to upload, download, and manage their files through a web browser.

## The Database Tier

The database tier uses MariaDB to store persistent application data, including user accounts, settings, and file metadata.

## Why Separate Them?

Separating the application and database into different containers makes the system easier to manage, update, and troubleshoot. It also allows each service to operate independently while communicating through a private Docker network.
