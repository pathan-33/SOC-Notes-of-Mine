# **Linux for Hackers**

## **Introduction to Linux**

Linux is an essential foundational skill for anyone interested in hacking. Understanding Linux is a prerequisite for many tasks in the hacking realm. This series aims to equip learners with the foundational knowledge needed to use Linux effectively. The content presented is applicable to everyone, regardless of background.

## **What is Linux?**

Linux is not merely an operating system; it is technically a kernel. An operating system (OS) is built on top of this kernel. Common distributions of Linux include:

- Parrot OS: An OS built specifically for hacking.
- Kali Linux
- Ubuntu
- CentOS
- Debian

The Linux kernel acts as an interface between hardware (CPU, RAM, hard drive) and the applications that run on the OS, such as hacking tools like Nmap.

### **Benefits of Using Linux**

1. **Open Source**: Linux is free to use and redistribute, allowing for the creation of various distributions.
2. **Performance**: Linux is typically faster than other operating systems.
3. **Security**: Linux is known for being more secure, making it the OS of choice for numerous websites and servers.
4. **Hacking Tools**: Most hacking tools are Linux-based, making it essential for hackers to be proficient in Linux.

## **The Linux Terminal**

While Linux has a graphical user interface (GUI), the true power of Linux is unlocked through the command line interface, known as the terminal. Users should familiarize themselves with terminal commands to gain efficiency and control over the system.

### **Basic Terminal Commands**

1. **pwd**: Print Working Directory
- Usage: Type pwd and hit enter.
- Function: Displays the full path of the current directory.
1. **ls**: List
- Usage: Type ls and hit enter.
- Function: Lists the contents of the current directory.
1. **cd**: Change Directory
- Usage: Type cd folder_name to move into a specific folder.
- Example: cd desktop changes the current directory to the Desktop folder.
- To go back to the previous directory, use cd ...

### **Example Usage of Commands**

1. Start by opening the terminal and entering the pwd command to see your current location in the filesystem.
2. Use the ls command to list the contents of your current directory, which may include folders like Documents, Downloads, and Desktop.
3. Navigate to the Desktop directory with the command cd desktop.
4. List the contents of the Desktop directory using ls.
5. To return to the previous directory, type cd .. and use pwd to confirm your location.

## **Understanding the Filesystem**

The Linux filesystem is structured hierarchically. The root directory, denoted as /, is the top level of the filesystem. From this root, various directories branch out, including /home, which contains user-specific directories.

### **Navigating the Filesystem**

- Use pwd to see your current location.
- Use ls to view the contents of the directory.
- Use cd to navigate through directories.
- To move back to the root directory, type cd /.

## **Conclusion**

We covered the basics of Linux, emphasizing its importance for hacking. We explored the differences between the Linux kernel and operating systems, the benefits of using Linux, and fundamental terminal commands. As you continue to learn about Linux, remember to practice these commands to build your proficiency.

For further exploration and understanding, consider engaging with Hack The Box Academy, which provides guided learning experiences tailored to IT security, including a deeper dive into Linux commands.
