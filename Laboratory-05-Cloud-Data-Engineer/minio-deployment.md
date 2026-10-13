
# MinIO Object Storage Deployment Documentation

## Overview
This document outlines the technical steps taken to deploy an S3-compatible object storage server (MinIO) using Docker in the KillerCoda environment, access its management console, and set up a dedicated storage bucket.

---

## Technical Configuration Steps

### 1. Deploying MinIO via Docker
To start the MinIO server in the background, map the necessary ports, and assign root credentials, the following Docker command was executed in the KillerCoda terminal:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
  -e "MINIO_ROOT_USER=cloudadmin" \
  -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
  pgsty/minio server /data --console-address ":9001"
