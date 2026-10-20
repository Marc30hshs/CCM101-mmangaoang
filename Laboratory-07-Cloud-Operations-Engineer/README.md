# Laboratory Activity 7: The Cloud Operations Engineer

## Mission Overview
This laboratory activity focuses on monitoring Linux server resources and observing the performance of a containerized web application using Docker.

## Objectives
- Check the host server's RAM, disk storage, and CPU activity.
- Deploy an Nginx web server using Docker.
- Generate HTTP requests and simulate a 404 error.
- Analyze application logs using Docker.
- Monitor container CPU, memory, and network usage.
- Document system health and application performance.

## Monitoring Commands Executed

| Command | Purpose |
|---|---|
| `free -h` | Check RAM usage |
| `df -h /` | Check root filesystem storage |
| `top` | Monitor CPU and running processes |
| `docker run -d --name clientwebsite -p 8080:80 nginx` | Deploy the Nginx container |
| `curl -i http://localhost:8080/` | Test the website |
| `curl -i http://localhost:8080/hidden-admin-page` | Generate an HTTP 404 error |
| `docker logs clientwebsite` | View application logs |
| `docker stats clientwebsite` | Monitor container metrics |

## Skills Learned
- Linux system monitoring
- Docker container deployment
- HTTP request testing
- Application log analysis
- Real-time resource monitoring
- Markdown documentation and GitHub portfolio management

## Screenshots
All evidence screenshots are stored in the `screenshots/` directory.

## Conclusion
This activity demonstrated how Linux and Docker monitoring tools help Cloud Operations Engineers evaluate server health, troubleshoot application errors, and observe container resource usage.

