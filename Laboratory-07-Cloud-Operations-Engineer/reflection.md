# Mission Reflection

In this laboratory activity, I learned that monitoring is an important part of cloud computing. Deploying an application is not enough because we also need to make sure that the server and application are working properly.

Checking the host server's resources is important even when containers are running perfectly. Containers depend on the host machine for CPU, memory, and disk storage. If the server runs out of resources, the application may become slow, stop responding, or crash. By using Linux commands such as `free -h`, `df -h /`, and `top`, I can check the server's condition before problems happen.

The `docker logs` command is also useful when a user reports that they cannot log into a web application. It allows me to inspect application messages and identify possible errors, failed requests, or other problems. By checking the logs, I can gather evidence and investigate the issue instead of guessing its cause.

I also learned the difference between logs and metrics. Logs show individual events and messages, such as successful requests and HTTP 404 errors. Metrics provide numerical information about performance, including CPU usage, memory consumption, and network activity. Both are important because logs explain what happened, while metrics help show how the system is performing.

Large enterprise companies can monitor thousands of containers using centralized monitoring tools such as Prometheus and Grafana. Prometheus collects and stores metrics, while Grafana displays the information through dashboards and visualizations. These tools help engineers detect unusual activity and investigate performance problems across many servers and containers.

Overall, this laboratory improved my ability to troubleshoot Linux environments. I gained practical experience in checking system resources, deploying an Nginx container, generating HTTP requests, examining application logs, and monitoring Docker metrics. I also learned the importance of recording actual results and keeping screenshots as evidence. These skills will help me understand how Cloud Operations Engineers maintain reliable and efficient cloud applications.
