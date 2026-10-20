# Container Observability Report

## Application Logs

The Docker logs command was used to inspect the HTTP requests received by the Nginx container.

### HTTP 404 Error Log
Copy and paste the actual log line showing the 404 response from the terminal here.

### Importance of Application Logs
Application logs help identify errors, failed requests, and unusual activities within an application. They allow Cloud Operations Engineers to investigate problems and determine the possible causes of service failures.

## Evidence
- `screenshots/docker-logs.png`
## Real-Time Container Metrics

The `docker stats` command was used to monitor the live resource consumption of the Nginx container.

- **Container Name:** clientwebsite
- **CPU Usage:** [Enter exact CPU percentage]
- **Memory Usage:** [Enter exact memory usage, such as 3.5MiB]
- **Network I/O:** [Enter the value shown in the terminal]

### Analysis
The metrics provide information about the container's resource consumption. Monitoring CPU and memory usage helps determine whether the application is operating efficiently and whether it may require additional resources during periods of high traffic.

## Evidence
- `screenshots/container-metrics.png`
