
# Cloud Storage Types Research

## Storage Comparison Table

| Storage Type | Description (How does it store data?) | Primary Use Case (What is it best used for?) | Cloud Provider Example |
| :--- | :--- | :--- | :--- |
| **Block Storage** | Splits data into raw, fixed-sized blocks, each with its own address. It acts like a raw hard drive attached to an operating system. | High-performance databases, virtual machine boot volumes, and transactional workloads requiring low latency. | AWS EBS (Elastic Block Store), Azure Disk Storage |
| **File Storage** | Organizes data into a hierarchical structure of files and folders within directories, shared over a network (NAS). | Shared file directories, user home directories, content management systems, and collaborative team environments. | AWS EFS (Elastic File System), Azure Files |
| **Object Storage** | Manages data as discrete units called "objects" bundled with metadata and a unique identifier, flatly stored in a repository rather than a hierarchy. | Storing massive amounts of unstructured data such as photos, videos, system backups, data lakes, and static website hosting. | AWS S3 (Simple Storage Service), Google Cloud Storage |

## Client Recommendation

Object storage is unquestionably the best choice for storing millions of user-uploaded photos for your application. Unlike block storage, which is tightly bound to individual servers and difficult to scale cost-effectively, object storage offers virtually infinite scalability and attaches rich metadata to every file. Furthermore, its flat namespace and RESTful API access make retrieving, managing, and serving web images to global users both fast and reliable.
