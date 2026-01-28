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

The following commands are fundamental for navigating and interacting with the Linux file system:

- 

**pwd (Print Working Directory):**

- **Purpose:** Displays the full path of the current directory you are in.
- **Example:**

```bash
pwd
```

Output might look like: `/home/user/documents`
- 

**ls (List):**

- **Purpose:** Lists the contents (files and subdirectories) of the current working directory.
- **Example:**

```bash
ls
```

Output might look like: `desktop downloads documents notes.txt`
- 

**cd (Change Directory):**

- **Purpose:** Changes your current working directory to a specified directory.
- **Syntax:** `cd [directory_name]`
- **Example (moving into a subdirectory):**

```bash
dc desktop  # Note: Correct command should be 'cd' not 'dc'
def change_directory_to_desktop():  # Pseudocode for clarity in markdown context  	cd('desktop')  # Actual command in terminal would be 'cd desktop'
def verify_current_directory():  	print(pwd())  # Should output '/home/user/89786/desktop'
def move_up_one_directory():  	cd('..')  # Moves up one level in hierarchy  
def move_to_root():  	cd('/')  # Moves to root directory  
def move_to_home():  	cd('~') or tcd()  # Moves to home directory ```
the correct command sequence would be:
desktop` after running this, `pwd` would show `/home/user/documents/desktop`.
e.g., moving into a subdirectory:
db cd desktop   # Correct syntax in terminal: 'cd desktop'
e.g., moving up one directory:
db cd ..   # Correct syntax: 'cd ..'
e.g., moving to root:
db cd /   # Correct syntax: 'cd /'
e.g., moving to home:
db cd ~ or just `cd`
and verifying location with `pwd`.
