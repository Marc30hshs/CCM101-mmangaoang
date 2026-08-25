
# Checkpoint 3 – Cloud Infrastructure Components

## 1. Compute Resources

**Linux Example:** CPU / Processor

**Purpose:**
The CPU acts as the main processing unit of the Linux system. It executes commands, runs programs, and handles the tasks requested by the user.

**Importance in Cloud Computing:**
Cloud applications need processing power to serve users and perform different workloads. Compute resources can also be increased or decreased depending on the workload.

**KillerCoda Connection:**
The CPU available in the KillerCoda Linux environment can be inspected with:

```bash
lscpu
```

This command provides details about the processor assigned to the environment.

---

## 2. Storage Resources

**Linux Example:** Disk Space / File System

**Purpose:**
Storage keeps important system files, applications, configurations, and other data even when they are not currently being used.

**Importance in Cloud Computing:**
Cloud services require storage to maintain application data, databases, files, and system information. Reliable storage helps prevent data loss and supports continuous access to information.

**KillerCoda Connection:**
The storage available in the Linux environment can be checked with:

```bash
df -h
```

This shows how much disk space is being used and how much remains available.

---

## 3. Networking Resources

**Linux Example:** Network Interface / IP Address

**Purpose:**
Networking allows the Linux environment to communicate with other systems and connect to external services.

**Importance in Cloud Computing:**
Networking is essential because cloud resources are connected through networks. It allows users to access applications, servers to communicate, and services to exchange data.

**KillerCoda Connection:**
KillerCoda provides network interfaces and an IP address that can be examined using:

```bash
hostname -I
ip addr
```

These commands help identify the network configuration of the Linux environment.

---

## 4. Operating System

**Linux Example:** Linux

**Purpose:**
The operating system manages the computer's hardware and provides the platform where applications, services, and commands can run.

**Importance in Cloud Computing:**
An operating system provides the foundation for cloud servers. Linux is commonly used because it is efficient, flexible, stable, and supports many server applications.

**KillerCoda Connection:**
KillerCoda provides a Linux environment that allows users to practice managing a cloud-like system through the terminal. Users can inspect hardware, storage, networking, and other system resources.

---

## Summary

The KillerCoda environment provides a practical example of how infrastructure components work together. **Compute** handles processing, **storage** keeps information, **networking** enables communication, and the **Linux operating system** coordinates these resources. These same components are fundamental building blocks of modern cloud infrastructure.
