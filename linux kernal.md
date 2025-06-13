# 🐧 Linux Kernel

The **Linux kernel** is the core part of the Linux operating system. It is a free, open-source, monolithic, Unix-like operating system kernel created by **Linus Torvalds** in 1991. It handles communication between hardware and software components, manages system resources, and enables multitasking and device control.

---

## 📚 Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Kernel Components](#kernel-components)
- [Kernel Versioning](#kernel-versioning)
- [Building the Kernel](#building-the-kernel)
- [Useful Resources](#useful-resources)
- [Conclusion](#conclusion)

---

## 🔍 Overview

The Linux kernel forms the foundation of many operating systems including Ubuntu, Debian, Fedora, Android, and countless others. It is:
- **Modular**: Uses loadable kernel modules (LKMs)
- **Portable**: Runs on a wide range of hardware platforms
- **Secure**: Implements permission systems, security modules, and namespaces
- **Scalable**: Powers everything from smartphones to supercomputers

---

## 🚀 Key Features

- Process Scheduling
- Virtual Memory Management
- Virtual File System (VFS)
- Device Drivers
- Networking (TCP/IP, IPv6, Netfilter)
- Security Modules (SELinux, AppArmor)
- Inter-Process Communication (IPC)

---

## 🧩 Kernel Components
**1. 🧱 Process Scheduler (Process Management)**

> Handles the **creation, scheduling, and termination** of processes and threads

> This supports the **multi-tasking and multi-threading**.

> Uses scheduling algorithms (like CFS - Completely Fair Scheduler) to decide which process runs on which CPU and for how long.

**2. 🧠 Memory Management**

> Manages **RAM and virtual memory (paging, swapping, memory mapping)**.

> Handles **allocation and deallocation** of memory for the processes

> This implement the virtual memory using **MMU (Memory management Unit)**

**3. 🧾 Virtual File System (VFS)**

> This provides the basic file operations: open, read, write, close

> Abstracts filesystem access so that the kernel can support multiple filesystem types like **ext4, XFS, Btrfs, FAT, NTFS, etc**.

**4. 📡 Network Stack**

> Implements the network protocols: **TCP/IP, UDP, ICMP etc**

> Supports IPv4, IPv6, firewalls (**via Netfilter**), traffic shaping, etc.

**5. 🔧 System Calls Interface**

> This is the interface which the **user-space application** interact with the kernal

> Also provides the access to the kernal functions (eg `read()`, `write()`, `exec()`).

**6. 🔄 Kernel Space vs User Space**

> Kernel space: Where all the components above reside.

> User space: Where applications and utilities run.

> Communication is done via system calls and APIs.

## 📊 Summary Table:

| Component             | Description                                               |
|-----------------------|-----------------------------------------------------------|
| **Scheduler**         | Allocates CPU time to processes                           |
| **Memory Manager**    | Manages RAM, virtual memory, swap                         |
| **VFS**               | Provides an abstraction layer over different filesystems  |
| **Device Drivers**    | Enable interaction with hardware                          |
| **Network Stack**     | Implements network protocols and communication            |
| **System Call Interface** | Gateway between userspace and kernel space           |
| **IPC Subsystem**     | Pipes, message queues, shared memory                      |
| **Security Subsystem**| Enforces access control and isolation                     |

---

## 🔢 Kernel Versioning

Linux kernel versions follow the format: `major.minor.patch`

Example:

* To check the verison: 
```bash
prajwal@prajwal-Inspiron-15-3567:~$ uname -r
6.11.0-8-generic


- `6`: Major version (architectural changes)
- `9`: Minor version (new features)
- `1`: Patch level (bug/security fixes)
```
---

## 🏗️ Building the Kernel

**1. Configure the Kernel**

``make menuconfig``

**2. Compile the Kernal**

``make -j$(nproc) ``

**3. Installing the modules and kernal**

``sudo make modules_install``

``sudo make install``

**4. Update Bootloader (GRUB)**

``sudo update-grub``

**5. Reboot into New Kernel**

``sudo reboot``

---

## 🌐 Useful Resources

| Resource                    | Link                                                                                                                                |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| Official Kernel Site        | [https://www.kernel.org](https://www.kernel.org)                                                                                    |
| Git Source Repository       | [https://git.kernel.org](https://git.kernel.org)                                                                                    |
| Kernel Newbies Guide        | [https://kernelnewbies.org](https://kernelnewbies.org)                                                                              |
| GeeksforGeeks Guide         | [https://www.geeksforgeeks.org/linux-unix/the-linux-kernel](https://www.geeksforgeeks.org/linux-unix/the-linux-kernel)              |                                                                                       |


---

## ✅ Conclusion

The Linux kernel is a powerful, flexible, and open-source core that drives many of the world's operating systems. Its modular design, strong community, and robust features make it a leading choice for developers, enterprises, and researchers.The Kernel has provided a wide range of features, for example, memory management, filesystem management, process management, device drive management and networking support. After understanding all this one can conclude that customizability and extensibility have made it the most popular choice for a computer system.
