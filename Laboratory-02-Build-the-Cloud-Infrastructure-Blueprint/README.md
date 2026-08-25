
# ☁️ Cloud Infrastructure Laboratory

## Mission Overview

This laboratory activity was designed to provide hands-on experience with the basic components of a cloud server. Using the **KillerCoda Linux environment**, I investigated system resources, examined the server configuration, compared major cloud providers, and created a simple cloud infrastructure design.

The main purpose of the laboratory was to connect Linux system administration concepts with real-world cloud infrastructure.

---

## Objectives

The laboratory aimed to:

* Identify the main resources available on a Linux cloud server.
* Investigate CPU, memory, storage, networking, and operating system information.
* Understand how Linux commands can be used for infrastructure monitoring.
* Compare equivalent infrastructure services from AWS, Microsoft Azure, and Google Cloud.
* Create a simple representation of a cloud infrastructure.
* Document technical findings using Markdown.

---

## Cloud Infrastructure Components

The following infrastructure components were examined during the laboratory:

| Component            | Example                 | Role                                       |
| -------------------- | ----------------------- | ------------------------------------------ |
| **Compute**          | Intel Xeon CPU          | Processes commands and workloads           |
| **Memory**           | 1.9 GiB RAM             | Temporarily holds active data and programs |
| **Storage**          | `/dev/vda1`             | Stores system files and application data   |
| **Networking**       | `enp1s0` / `172.30.1.2` | Provides network connectivity              |
| **Operating System** | Ubuntu 24.04.4 LTS      | Manages the server and its resources       |
| **File Systems**     | ext4 / tmpfs            | Organizes and manages stored data          |

These components work together to form the basic foundation of a cloud computing environment.

---

## Tools Used

The following tools and platforms were used throughout the laboratory:

* **KillerCoda** – Provided the Linux-based cloud server environment.
* **Linux Terminal** – Used to investigate and manage system resources.
* **Draw.io** – Used to design the cloud infrastructure diagram.
* **Markdown** – Used to create and organize technical documentation.
* **AWS Documentation** – Used to research Amazon cloud services.
* **Microsoft Azure Documentation** – Used to research Azure services.
* **Google Cloud Documentation** – Used to research GCP services.

---

## Linux Commands Executed

Several Linux commands were used to collect information from the server.

### System Information

```bash
cat /etc/os-release
uname -r
lscpu
free -h
```

### Storage Information

```bash
df -h
findmnt
```

### Host and Network Information

```bash
hostname
hostname -I
ip -br addr
```

These commands made it possible to inspect the server without relying on a graphical interface.

---

## Skills Learned

Through this laboratory, I developed the following skills:

* Basic Linux system investigation
* CPU and memory resource identification
* Disk and file system inspection
* Network interface and IP address identification
* Understanding of cloud infrastructure components
* Comparing services across different cloud providers
* Creating basic cloud architecture diagrams
* Writing technical documentation using Markdown
* Reading and interpreting terminal output
* Connecting Linux administration concepts to cloud computing

---

## Challenges Encountered

One challenge was understanding the large amount of information returned by Linux commands. Some commands displayed more technical details than were immediately needed, so the relevant information had to be identified carefully.

Another challenge was comparing AWS, Azure, and GCP because each provider uses different service names for similar infrastructure. For example, **Amazon EC2, Azure Virtual Machines, and Google Compute Engine** all provide compute capabilities but use different interfaces and terminology.

Creating the cloud infrastructure diagram was also challenging because the required components needed to be arranged clearly while still showing how they communicate with each other.

---

## Final Reflection

This laboratory showed that cloud infrastructure is not simply about accessing a remote server. It involves several interconnected resources, including **compute, memory, storage, networking, and operating systems**. By investigating these components through KillerCoda, I gained a better understanding of what happens underneath cloud services and how basic Linux administration skills can be applied to cloud environments.

> **Key Takeaway:** Understanding the infrastructure behind the cloud makes it easier to understand how cloud services are built, connected, and managed.
