

# Mission Reflection

This laboratory activity helped me understand how Docker Compose makes cloud deployment easier and more organized. Instead of starting each container manually and entering many commands, I could define the application and database services in one YAML file. With a single command, Docker Compose could create and start the containers. This saves time, reduces repetitive work, and makes deployment easier to repeat.

I also learned that YAML indentation is very important. If I use incorrect spacing or a tab instead of spaces, the configuration may produce an error or fail to work as expected. This taught me to check the structure of my configuration file before deploying the application.

Environment variables were important in this activity because they provided the database name, username, password, and hostname required by Nextcloud to connect to MariaDB. These settings helped the two containers communicate. I also learned that credentials written directly in a Compose file are suitable only for a basic lab and should be handled more securely in production.

Deploying Nextcloud in just a few minutes was a good experience because I saw how different services can work together to create a private cloud storage system. I learned that successful deployment requires more than writing code. I also needed to check container status, access the application through a browser, review logs when necessary, and shut down the services properly.

Since Mission 1, my understanding of cloud computing has developed from learning basic infrastructure concepts to deploying and managing applications. I now understand that cloud engineers need technical skills, planning, automation, testing, and documentation. This mission showed me why Infrastructure as Code is valuable because it makes deployments more consistent and easier for other engineers to understand. Overall, this activity improved my confidence in using Linux, Docker, YAML, and technical documentation.
