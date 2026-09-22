
# Docker Deployment

## Docker Image and Container Deployment

### 1. Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the official Nginx image from Docker Hub so it can be used to create a container.

---

### 2. Run the Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

This command creates and starts the Nginx container in detached mode and maps port 8080 on the host to port 80 inside the container.

---

### 3. Verify the Nginx Web Server

```bash
curl http://localhost:8080
```

This command sends an HTTP request to the Nginx web server and displays the returned HTML content in the terminal.

---

# Container Lifecycle

### 4. List Running Containers

```bash
docker ps
```

This command displays all Docker containers that are currently running.

---

### 5. Stop the Running Container

```bash
docker stop nginx-server
```

This command stops the running `nginx-server` container.

---

### 6. Verify the Container is Stopped

```bash
docker ps
```

This command confirms that the `nginx-server` container is no longer running.

To view the stopped container, use:

```bash
docker ps -a
```

This command displays all containers, including stopped containers.

---

### 7. Remove the Container

```bash
docker rm nginx-server
```

This command permanently removes the stopped `nginx-server` container from the Docker environment.

---

### 8. Verify Container Removal

```bash
docker ps -a
```

This command confirms that the `nginx-server` container has been removed.

---

## Docker Command Summary

| Command | Purpose |
|---|---|
| `docker pull nginx` | Downloads the Nginx image from Docker Hub. |
| `docker run -d --name nginx-server -p 8080:80 nginx` | Creates and runs the Nginx container. |
| `curl http://localhost:8080` | Tests the Nginx web server. |
| `docker ps` | Lists running containers. |
| `docker stop nginx-server` | Stops the Nginx container. |
| `docker ps -a` | Lists all containers, including stopped containers. |
| `docker rm nginx-server` | Removes the stopped Nginx container. |

## Screenshot

The container lifecycle commands were executed in the KillerCoda Docker playground.

![Container Lifecycle](screenshots/container-lifecycle.png)
