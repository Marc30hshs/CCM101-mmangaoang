# Research: Types of Cloud Storage

## Comparison of Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-sized blocks that can be accessed independently. | Virtual machine disks and databases. | AWS EBS |
| File Storage | Stores data in files organized into folders and directories. | Shared folders and file-sharing systems. | AWS EFS |
| Object Storage | Stores data as objects with unique identifiers and metadata inside buckets. | Photos, videos, backups, and unstructured data. | AWS S3 |

## Recommendation to the Client

Object Storage is the best choice for storing user-uploaded images because it can handle large amounts of unstructured data and scale as the application grows. Each image is stored as an object with its own identifier and metadata, making it easier to organize and retrieve files. It is also suitable for applications that need reliable access to images.
