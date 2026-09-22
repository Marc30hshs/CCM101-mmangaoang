
# Mission Reflection

## 1. How does the boot time and setup process of a Docker container compare to installing an operating system on a Virtual Machine?

A Docker container is much faster to start compared to installing and booting an operating system on a Virtual Machine. A VM needs to install a complete operating system and allocate resources such as RAM, CPU, and storage. In Docker, the container uses the host operating system's kernel, so it does not need a complete operating system. Because of this, a Docker container can usually start within seconds.

## 2. Why is port mapping (-p 8080:80) necessary when running a web server inside a container?

Port mapping allows the host machine to communicate with the web server inside the container. In this activity, `-p 8080:80` maps port 8080 on the host to port 80 inside the Nginx container. This allowed me to access the Nginx web server using `curl http://localhost:8080`. Without port mapping, the service inside the container would not be directly accessible through that host port.

## 3. What happens to the data inside a container when you use the docker rm command?

The `docker rm` command removes a stopped container from Docker. Any data stored only in the container's writable layer is removed together with the container. This means important data should not be stored only inside a temporary container. Docker volumes or other persistent storage can be used when data needs to remain available after the container is removed.

## 4. How do you think containerization changes the way software developers and IT operations teams work together (DevOps)?

Containerization can improve cooperation between developers and IT operations teams because they can use the same application environment. Developers can test an application inside a container, while operations teams can deploy the same container in another environment. This can reduce differences between development and production environments and make deployment more consistent.

## 5. How is your GitHub portfolio evolving?

My GitHub portfolio is becoming more organized as I add each laboratory activity. In this laboratory, I added Docker deployment, container management, technical documentation, and screenshots of my work. These activities show my progress in learning cloud computing and practical IT skills. I can continue improving my portfolio by adding more projects, documentation, and evidence of the skills I learn.
