
# Mission 5 – Cloud Data Engineer Reflection

### 1. Why is object storage better suited for storing millions of photos compared to a traditional block storage hard drive?

Object storage is better for millions of photos because it can store large amounts of unstructured data and scale as the application grows. Each photo has its own identifier and metadata, making files easier to organize and retrieve.

### 2. How did using Docker make it easier to deploy the MinIO storage server?

Docker made deployment easier because it allowed me to run MinIO in a container without manually installing all its components. I could also configure the ports and login credentials using environment variables.

### 3. What is a "bucket" in the context of cloud storage?

A bucket is a container used to organize and store objects or files in object storage. In this activity, the bucket name was `client-photos`.

### 4. How do you think large enterprise companies ensure their object storage data is not lost if the physical server crashes?

Large companies use backups, data replication, and redundancy to protect their files. They keep copies of data across different servers or locations so they can recover files if a server fails.

### 5. How is your confidence in navigating the Linux command line growing?

My confidence in using Linux is improving because I learned how to run Docker commands, check container status, and view logs. I am becoming more comfortable using the command line to deploy and manage cloud services.
