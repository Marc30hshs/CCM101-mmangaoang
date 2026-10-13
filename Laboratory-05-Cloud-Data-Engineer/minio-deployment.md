# MinIO Deployment Documentation

## 1. Overview
This laboratory demonstrates how to deploy MinIO object storage using Docker in a KillerCoda Ubuntu environment.

## 2. Docker Command Used

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
  -e "MINIO_ROOT_USER=cloudadmin" \
  -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
  pgsty/minio server /data --console-address ":9001"
```

## 3. Port Configuration
- **Port 9000:** MinIO S3-compatible API.
- **Port 9001:** MinIO Web Console.

## 4. Login Credentials
- **Username:** `cloudadmin`
- **Password:** `CloudNova2026!`

## 5. Environment Variables
The `-e` flag in Docker is used to set environment variables inside the container.

- `MINIO_ROOT_USER` sets the administrator username.
- `MINIO_ROOT_PASSWORD` sets the administrator password.

These variables configure the credentials used to access the MinIO server.

## 6. Bucket Created
The bucket created for this laboratory is named `client-photos`.

## 7. File Upload
A sample image or text file was uploaded to the `client-photos` bucket through the MinIO Web Console.

## 8. Screenshots
- `screenshots/minio-deployed.png` – Shows the running MinIO container.
- `screenshots/minio-bucket-upload.png` – Shows the bucket and uploaded file.

## 9. Conclusion
MinIO was deployed using Docker and configured through environment variables. The Web Console was accessed through port 9001, and the `client-photos` bucket was used to store a sample file.
