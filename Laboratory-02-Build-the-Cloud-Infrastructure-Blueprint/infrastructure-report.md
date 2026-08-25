
# Checkpoint 2 – Cloud Server Investigation

## 1. Overview

For this checkpoint, I investigated the Linux server provided through the **KillerCoda terminal**. The investigation focused on identifying the server's operating system, kernel, computing resources, memory, storage, mounted file systems, hostname, and network configuration.

---

## 2. Investigation Results

| Infrastructure Component | Finding                                                    |
| ------------------------ | ---------------------------------------------------------- |
| **Operating System**     | Ubuntu 24.04.4 LTS                                         |
| **Kernel Version**       | 6.8.0-138-generic                                          |
| **CPU Model**            | Intel Xeon E312xx (Sandy Bridge, IBRS update)              |
| **CPU Cores**            | 2 CPU cores                                                |
| **Total RAM**            | 1.9 GiB                                                    |
| **Disk Capacity**        | 19 GB primary disk (`/dev/vda1`)                           |
| **Hostname**             | ubuntu                                                     |
| **IP Address**           | 172.30.1.2                                                 |
| **Primary File System**  | ext4                                                       |
| **Mounted File Systems** | `/`, `/run`, `/dev/shm`, `/run/lock`, `/boot`, `/boot/efi` |

> **Note:** The CPU output shows the processor model but does not explicitly display the CPU count in the captured results. The environment can be verified with `lscpu | grep '^CPU(s):'` if an exact core count is required.

---

## 3. Operating System

The server is running **Ubuntu 24.04.4 LTS**, a Linux-based operating system commonly used for servers and cloud environments.

The operating system provides the basic platform for managing hardware resources, executing commands, and running applications.

```text
PRETTY_NAME="Ubuntu 24.04.4 LTS"
```

---

## 4. Kernel Version

The server uses kernel version:

```text
6.8.0-138-generic
```

The Linux kernel is responsible for managing important system resources such as the CPU, memory, storage devices, and network interfaces.

---

## 5. CPU

The identified processor is:

```text
Intel Xeon E312xx (Sandy Bridge, IBRS update)
```

The Xeon processor provides the computing power required to execute commands and run services inside the Linux environment.

---

## 6. Memory

The system has approximately **1.9 GiB of total RAM**.

```text
Total RAM: 1.9 GiB
Used:      414 MiB
Available: 1.5 GiB
```

RAM temporarily stores data and programs that are actively being used by the operating system and applications.

---

## 7. Disk Capacity

The main disk is:

```text
/dev/vda1
```

with approximately:

```text
Total: 19G
Used:  5.4G
Free:  13G
```

The primary file system is mounted at `/` and uses the **ext4** file system.

---

## 8. Mounted File Systems

The investigation identified the following mounted file systems:

| Mount Point | Device / Source | File System |
| ----------- | --------------- | ----------- |
| `/`         | `/dev/vda1`     | ext4        |
| `/dev/shm`  | tmpfs           | tmpfs       |
| `/run`      | tmpfs           | tmpfs       |
| `/run/lock` | tmpfs           | tmpfs       |
| `/boot`     | `/dev/vda16`    | ext4        |
| `/boot/efi` | `/dev/vda15`    | EFI         |

These mounted file systems provide different areas for the operating system, temporary files, boot files, and system operations.

---

## 9. Hostname

The hostname of the server is:

```text
ubuntu
```

The hostname identifies the Linux machine within its environment and can be useful when managing multiple servers.

---

## 10. Network Configuration

The primary IP address identified is:

```text
172.30.1.2
```

The system also has a Docker network address:

```text
172.17.0.1
```

The network interfaces reported by the system are:

| Interface | Status  | Address       |
| --------- | ------- | ------------- |
| `lo`      | UNKNOWN | 127.0.0.1     |
| `enp1s0`  | UP      | 172.30.1.2/24 |
| `docker0` | DOWN    | 172.17.0.1/16 |

The `enp1s0` interface is the primary active network interface, while `docker0` is associated with Docker networking.

---

## 11. Conclusion

The KillerCoda investigation provided a practical view of a Linux-based cloud server. The environment runs Ubuntu 24.04.4 LTS with an Intel Xeon processor, approximately 1.9 GiB of RAM, a 19 GB primary disk, several mounted file systems, and an active network interface using the `172.30.1.2` address.

This investigation demonstrates how basic Linux commands can be used to identify the infrastructure resources available on a cloud-based server.

## Commands Used

```bash
cat /etc/os-release
uname -r
lscpu
free -h
df -h
findmnt
hostname
hostname -I
ip -br addr
```

## Screenshot Evidence

Screenshots of the KillerCoda terminal investigation should be included with this report as evidence of the collected system information.
