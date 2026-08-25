
# Cloud Provider Comparison

## Introduction

Cloud providers offer many of the same basic infrastructure capabilities, but they organize and name their services differently. This comparison focuses on four important areas: **compute, storage, networking, and identity and access management (IAM)**.

## Core Infrastructure Service Comparison

| Infrastructure Component         | Amazon Web Services (AWS)                                                                                           | Microsoft Azure                                                                                                                     | Google Cloud Platform (GCP)                                                                                                  |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| **Compute**                      | **Amazon EC2** – Provides virtual servers that can run applications and workloads.                                  | **Azure Virtual Machines** – Provides scalable virtual machines for running applications and operating systems.                     | **Compute Engine** – Provides configurable virtual machines for running workloads in Google Cloud.                           |
| **Storage**                      | **Amazon S3** – Object storage used for files, backups, application data, and other objects.                        | **Azure Blob Storage** – Object storage designed for large amounts of unstructured data.                                            | **Cloud Storage** – Object storage for storing and accessing data using buckets and objects.                                 |
| **Networking**                   | **Amazon VPC** – Creates an isolated virtual network where AWS resources can be placed and connected.               | **Azure Virtual Network (VNet)** – Provides private networking between Azure resources and supports connectivity to other networks. | **Virtual Private Cloud (VPC)** – Provides networking for Google Cloud resources, including IP ranges, subnets, and routing. |
| **Identity & Access Management** | **AWS IAM** – Controls which users, roles, and services can access AWS resources and what actions they can perform. | **Microsoft Entra ID + Azure RBAC** – Manages identities and controls access to Azure resources through roles and permissions.      | **Cloud IAM** – Uses identities, roles, and permissions to control access to Google Cloud resources.                         |

AWS describes VPC as a logically isolated virtual network where resources such as EC2 instances can be deployed, while AWS IAM controls authentication and authorization through identities, roles, and policies. Google Cloud similarly uses IAM roles and permissions to control access to Compute Engine and other resources.

## Guide Questions

### 1. Which cloud provider offers the broadest range of services?

**AWS** is generally considered to have the broadest service portfolio among the three major providers. It provides a very large collection of services covering computing, storage, networking, databases, security, analytics, containers, AI, and many other areas, giving organizations many options for building different types of systems.

### 2. Which cloud platform would you recommend for an organization that primarily uses Microsoft products? Why?

I would recommend **Microsoft Azure** because it integrates naturally with Microsoft's ecosystem. Organizations already using products such as Windows Server, Microsoft 365, Active Directory-related technologies, and other Microsoft services can benefit from Azure's integration and identity management capabilities.

### 3. Which platform is widely recognized for Artificial Intelligence, Machine Learning, and Kubernetes services?

**Google Cloud Platform (GCP)** is widely recognized for its strengths in AI, machine learning, and Kubernetes technologies. Google has extensive experience in these areas, and its cloud platform provides services and infrastructure designed for developing, training, and deploying modern AI/ML workloads and containerized applications.

### 4. What similarities did you observe among the three cloud providers?

The three providers offer equivalent building blocks even though their service names are different. Each provides **virtual computing, scalable storage, private networking, and identity/access management**, allowing organizations to build complete cloud infrastructures using similar fundamental concepts.

## Conclusion

AWS, Azure, and GCP use different names and interfaces, but their core infrastructure concepts are closely related. Understanding these similarities makes it easier for a cloud engineer to transfer knowledge from one platform to another instead of learning every provider completely from scratch.

### Official Documentation

* **AWS:** Amazon EC2, Amazon S3, Amazon VPC, and AWS IAM
* **Microsoft Azure:** Azure Virtual Machines, Azure Blob Storage, Azure Virtual Network, and Microsoft Entra ID
* **Google Cloud:** Compute Engine, Cloud Storage, VPC, and Cloud IAM
