# Cloud Infrastructure Components

## Compute Resources
- **Purpose:** Provides processing power to run applications and workloads.
- **Importance in cloud:** Compute is what customers rent and scale on demand (VMs, containers).
- **In KillerCoda:** The vCPUs from `nproc`/`lscpu` and the RAM from `free -h`.

## Storage Resources
- **Purpose:** Persistent storage of data, files, and applications.
- **Importance in cloud:** Durability, backup, and scalability of data.
- **In KillerCoda:** The disk and file systems from `df -h` and `lsblk`.

## Networking Resources
- **Purpose:** Connects systems to each other and to the internet.
- **Importance in cloud:** Enables access, isolation, and communication between services.
- **In KillerCoda:** The interface, IP address, and hostname from `ip addr` and `hostname -I`.

## Operating System
- **Purpose:** Manages hardware and provides the environment for software.
- **Importance in cloud:** Base layer for every VM and container workload.
- **In KillerCoda:** The Linux distribution and kernel from `/etc/os-release` and `uname -r`.
