# Linux Fundamentals for Security Analysts

This README documents my learning of Linux fundamentals from a **SOC Analyst (L1)** perspective.  
The focus is on understanding how Linux systems work, why they are widely used in enterprises, and how they are involved in real-world security monitoring and investigations.

---

## Introduction to Linux

Linux is often misunderstood as a complete operating system. In reality, **Linux is a kernel**, which is the core component responsible for managing CPU, memory, hardware devices, and running processes.

A complete Linux operating system is built by combining the Linux kernel with:

- A shell for command-line interaction
- Device drivers for hardware support
- System utilities such as text editors and networking tools
- Package managers to install and update software
- A graphical user interface (GUI), if required

A simple way to understand this is to think of the kernel as a car engine, while the Linux operating system is the entire car.

---

## Linux Distributions (Distros)

A Linux distribution is a packaged version of Linux that includes the kernel along with software tools, system utilities, and configuration defaults.

Distributions mainly differ in:

- Package manager used
- Default system utilities
- Desktop environment
- Pre-installed tools and security focus

### Common Linux Distributions

- **Ubuntu** – Beginner-friendly, widely used on servers and cloud platforms  
- **Debian** – Stable, secure, and lightweight  
- **Red Hat Enterprise Linux (RHEL)** – Enterprise-focused with commercial support  
- **Rocky Linux** – Community-supported alternative to CentOS  
- **Kali Linux** – Designed for penetration testing and security assessments  
- **Parrot OS** – Security-focused with privacy tools  
- **REMnux** – Specialized for malware analysis and DFIR  

All distributions use the Linux kernel, but they differ in tools, configuration, and purpose.

---

## Why Linux Is Important for Cybersecurity

Linux is critical in cybersecurity for several reasons:

- Most enterprise servers and cloud infrastructure run Linux  
- Logs from Linux systems are heavily used in SOC investigations  
- Many attack tools and command-and-control servers run on Linux  
- Most security tools are designed for or run best on Linux  

### Examples of Linux-based security tools:

- **IDS:** Suricata, Zeek  
- **Endpoint visibility:** osquery  
- **DFIR tools:** Velociraptor  

Understanding Linux is mandatory for SOC analysts, blue teamers, and DFIR professionals.

---

## Linux vs Windows: Key Differences

| Feature             | Windows             | Linux                    |
|--------------------|-------------------|-------------------------|
| Process management  | Task Manager (GUI) | ps, top, htop           |
| Service management  | services.msc       | systemctl, service      |
| User privileges     | Administrator      | sudo, root              |
| File system         | Drive letters (C:, D:) | Single tree starting at / |
| Permissions         | ACL-based          | rwx for owner, group, others |
| File execution      | Extension-based    | Permission-based        |

---

## Linux File System Hierarchy

Linux uses a single hierarchical directory structure starting from the root directory `/`.

### Important Directories

- `/` – Root of the file system  
- `/bin` – Essential user commands  
- `/sbin` – System administration commands  
- `/home` – Home directories for users  
- `/var` – Logs and variable data  
- `/etc` – Configuration files  
- `/tmp` – Temporary files  
- `/usr` – User-installed programs  
- `/opt` – Optional software packages  
- `/mnt` – Temporary mount points  
- `/proc` – Virtual file system for processes  
- `/sys` – Kernel and hardware information  

---

## Essential Linux Commands

### Navigation and Information

- `pwd` – Show current directory  
- `ls` – List directory contents  
- `ls -la` – Detailed list including hidden files  
- `cd <dir>` – Change directory  
- `cd ..` – Move up one level  
- `cd ~` – Go to home directory  
- `tree` – Display directory structure  

### File and Directory Operations

- `touch file` – Create an empty file  
- `cat file` – Display file content  
- `nano file` – Edit file using Nano editor  
- `vi file` – Edit file using Vi editor  
- `mkdir dir` – Create directory  
- `mkdir -p parent/child` – Create nested directories  
- `cp src dest` – Copy files  
- `mv src dest` – Move or rename files  
- `rm file` – Delete file  
- `rm -r dir` – Delete directory recursively  
- `less file` – View file page by page  
- `head file` – View first 10 lines  
- `tail file` – View last 10 lines  
- `tail -f file` – Monitor file in real time  

---

## Users, Groups, and Permissions

Linux is a multi-user operating system. Every file and process belongs to a user and a group.

### User Types

- **Root** – Full administrative access  
- **System users** – Used by services (nginx, mysql)  
- **Normal users** – Human users  

### User and Group Information

- `whoami` – Show current user  
- `cat /etc/passwd` – List all users  
- `cat /etc/group` – List all groups  

Each user has a **UID**, and each group has a **GID**.

---

## Linux Permissions

Permissions are assigned to:

- Owner  
- Group  
- Others  

Permission types:

- **Read (r)** – View file or list directory  
- **Write (w)** – Modify file or directory  
- **Execute (x)** – Run file or enter directory  

Example permission string:

- **Owner:** read, write, execute  
- **Group:** read, execute  
- **Others:** read  

---

## sudo Command

The `sudo` command allows users to execute commands with elevated privileges.

### Examples:

- `sudo <command>` – Run command as root  
- `sudo useradd username` – Add a new user  
- `sudo usermod -aG sudo username` – Grant sudo access  

---

## Changing Permissions with chmod

Permissions can be modified using **octal notation**.

**Permission values:**

- Read = 4  
- Write = 2  
- Execute = 1  

### Examples:

- `chmod 755 file` – Owner full access, others read and execute  
- `chmod 666 file` – Everyone read and write  

---

## System Monitoring

### Process Monitoring

- `top` – Real-time process monitoring  
- `htop` – Enhanced version of top  
- `ps aux` – Snapshot of all processes  

### Memory Monitoring

- `free -h` – View RAM and swap usage  

### Disk Monitoring

- `df -h` – View disk usage  

### Network Monitoring

- `ip a` – View network interfaces  
- `netstat` – View network connections  
- `ss -tulpn` – Modern alternative to netstat  

---

## Linux Video Tutorial

Watch this video for a practical walkthrough of Linux basics:

https://youtu.be/p3ZatIUpMP4

> *Note: Click the link above to watch the video on YouTube.*
