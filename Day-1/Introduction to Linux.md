# **Linux for Hackers: Foundations**

## **Introduction to Linux**

Linux is a foundational skill for anyone interested in hacking, IT, or general computer knowledge. It's an open-source operating system that offers speed, security, and flexibility.

### **What is Linux?**

- **Kernel vs. Operating System:** While commonly referred to as an operating system, Linux is technically a kernel. The kernel is the core component of an operating system that interfaces with the hardware.
- **Distributions (Distros):** Operating systems built on top of the Linux kernel are called distributions or "distros." Examples include Parrot OS, Kali Linux, Ubuntu, and CentOS. Each distro may have different features and target audiences.
- **Parrot OS:** The specific distribution used in this course is Parrot OS, which is designed for hacking and security professionals.

### **Why Use Linux?**

- **Open Source:** Linux is free to use, modify, and distribute. This fosters a large community and rapid development.
- **Speed and Performance:** Linux is generally faster and more efficient than other operating systems.
- **Security:** Linux is known for its robust security features.
- **Prevalence:** The majority of web servers and a significant portion of the internet's infrastructure run on Linux, making it essential for cybersecurity professionals.
- **Hacking Tools:** Most popular hacking and penetration testing tools are developed for or primarily run on Linux.

## **The Linux Terminal**

While Linux has graphical user interfaces (GUIs), its true power is unlocked through the command-line interface (CLI), also known as the terminal.

### **Accessing the Terminal**

In the provided Hack The Box Academy lab, the terminal can be accessed by clicking on its icon on the desktop.

### **Essential Terminal Commands**

The following commands are fundamental for navigating and interacting with the Linux file system.

- 

**pwd (Print Working Directory):**

- **Purpose:** Displays the full path of the current directory you are in.
- **Example:**

```
pwd

```

Output might look like: /home/user/documents

- 

**ls (List):**

- **Purpose:** Lists the contents (files and subdirectories) of the current working directory.
- **Example:**

```
ls

```

Output might look like: desktop downloads documents notes.txt

- 

**cd (Change Directory):**

- **Purpose:** Changes your current working directory to a specified directory.
- **Syntax:** cd [directory_name]
- **Example (moving into a subdirectory):**

```
cd desktop

```

After running this, pwd would show /home/user/documents/desktop.

- **Example (moving up one directory):**
- **Purpose:** Navigates to the parent directory of the current directory.
- **Syntax:** cd ..
- **Example:** If you are in /home/user/documents/desktop, running cd .. will move you to /home/user/documents.
- **Example (moving to the root directory):**
- **Purpose:** Navigates to the root of the file system.
- **Syntax:** cd /
- **Example:**

```
cd /

```

After running this, pwd would show /.

- **Example (moving to the home directory):**
- **Purpose:** Navigates directly to your user's home directory.
- **Syntax:** cd ~ or simply cd
- **Example:**

```
cd ~

```

This will take you to /home/your_username.

### **Navigating the File System Hierarchy**

Linux uses a hierarchical file system structure, starting from the root directory (/).

- **Root Directory (/):** The topmost directory in the file system. All other directories and files are located under the root.
- **Home Directory (/home/username):** Each user typically has a dedicated home directory where their personal files and settings are stored.

### **Example Navigation Scenario**

Let's say you start in your home directory:

1. 

**Check your current location:**

```
pwd

```

Output: /home/user/89786 (The 89786 is an example of a username part in the lab)

1. 

**List the contents of your home directory:**

```
ls

```

Output: desktop downloads documents templates Postman

1. 

**Change into the desktop directory:**

```
cd desktop

```

1. 

**Verify you are in the desktop directory:**

```
pwd

```

Output: /home/user/89786/desktop

1. 

**List the contents of your desktop directory:**

```
ls

```

Output: (Lists files and folders present on your virtual desktop)

1. 

**Go back up to the parent directory (your home directory):**

```
cd ..

```

1. 

**Verify you are back in your home directory:**

```
pwd

```

Output: /home/user/89786

1. 

**Go all the way back to the root directory:**

```
cd /

```

1. 

**Verify you are at the root:**

```
pwd

```

Output: /

1. 

**List the contents of the root directory:**

```
ls

```

Output: bin dev etc home lib media mnt opt proc root run sbin srv sys tmp usr var (This is a typical structure, though it can vary slightly).
