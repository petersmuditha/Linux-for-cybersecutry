# 🐧 Linux Fundamentals: System Administration & Security

## Project Description
This repository documents my training in **Linux Fundamentals** via TryHackMe. The project focuses on mastering the Linux command-line interface (CLI) to perform system audits, manage files, and understand identity security. This documentation serves as a professional portfolio for Identity and Access Management (IAM) and Technical Writing roles.

## 🧭 what is it ?

Linux is the "engine" that runs most of the world's servers. Unlike Windows, it's an extremely modular open-source system. Imagine Linux as a house where you can decide exactly where to place each brick, making it much more difficult to break into if built well.

---

## 🚨 Projects & Use Cases (TryHackMe-based)

- Linux Filesystem Exploration	Linux Fundamentals Part 1	cd, ls, pwd, cat, find	Practical application of commands to navigate the directory structure of a Linux system and locate specific files.

- Introduction to Shell Operators]	Linux Fundamentals Part 1	&, &&, >, >>	Hands-on examples of running commands in the background and redirecting command output to automate simple tasks.
  
- User and Permission Management	Linux Fundamentals Part 2	ls -lh, chmod, file, User/Group concepts	Practical demonstration of how to view and modify access permissions for files and directories — a key security concept.

- Remote Administration via SSH	Linux Fundamentals Part 2	ssh, whoami, basic network commands	Walkthrough on establishing a secure SSH connection to a remote machine and executing administration commands, simulating server management.

- Pattern Searching & Log Analysis 101	Linux Fundamentals Part 1	grep, find, output redirection	Using grep and find to search for specific strings within files — a foundational skill for starting to analyze system logs.

> 🔒 *All data used in these projects is 100% synthetic and generated in isolated lab environments (TryHackMe rooms, custom VMs). No real customer or company data is ever used.*

---

## 📚 Why is it vital to our business ?

Stability and Performance: A Linux server can remain on for years without ever needing a reboot, ensuring our services are always online.Granular Security: Thanks to the permissions system, we can ensure that an employee (or hacker) can only see the files strictly necessary, isolating any potential threats.

Cost Efficiency: We don't pay expensive licenses for each server, allowing us to invest that budget in other areas of cybersecurity.

---

## 🛡️ How do we keep the system secure?

(Best Practices)
Principle of Least Privilege: We never use the "Root" user (the super-administrator) for daily operations. We use the sudo command only when absolutely necessary.

Permission Management: We constantly monitor who can "Read, Write, or Execute" (chmod) sensitive company files.

Constant Updates: We use package managers (such as apt) to immediately apply security patches as soon as vulnerabilities are discovered. 
Linux is often perceived as more intimidating or complex than familiar operating systems like *Windows*. However, both platforms offer unique strengths: while Windows focuses on user-friendliness, Linux stands out for being **extremely lightweight**, highly customizable, and robust.


## ⌨️ Essential Interaction: Basic Commands

Once we understand the importance of Linux, the next step is learning how to communicate with the system via the Command Line Interface (CLI). Below are two fundamental commands for any security professional.

### 1. `ls` (List)
The `ls` command displays the names of files and directories in your current location.
* **Why it matters:** It is the first step in auditing a system. Using `ls` allows a security analyst to see hidden files and check file permissions.

  ![image alt](https://github.com/petersmuditha/Linux-for-cybersecutry/blob/0d8ed979dd37fe43dcf48b0d73b9e676b0888044/Cattura5.PNG)


### 2. `cd` (Change Directory)
The `cd` command allows you to move between different directories in the filesystem.
* **Why it matters:** You must be able to navigate to sensitive areas, such as `/etc` (configuration) or `/var/log` (audit logs), to perform security checks.

  ![image alt](https://github.com/petersmuditha/Linux-for-cybersecutry/blob/0d8ed979dd37fe43dcf48b0d73b9e676b0888044/Cattura6.PNG)

### 3. `cat` (Concatenate)
The `cat` command reads the content of a file and displays it in the terminal.
* **Why it matters:** It allows you to inspect the contents of configuration files (like `/etc/passwd`) quickly without using an editor that might accidentally modify them.

  ![image alt](https://github.com/petersmuditha/Linux-for-cybersecutry/blob/0d8ed979dd37fe43dcf48b0d73b9e676b0888044/Cattura7.PNG)

### 4. `whoami` (Who Am I)
This command prints the username associated with the current session.
* **Why it matters:** In **Identity Management (IAM)**, verifying which user you are is crucial. It ensures you are not performing tasks as `root` unless absolutely necessary, following the **Principle of Least Privilege**.

![image alt](https://github.com/petersmuditha/Linux-for-cybersecutry/blob/0d8ed979dd37fe43dcf48b0d73b9e676b0888044/Cattura2.jpg)

  ### 5. `echo` (Echo)
The `echo` command prints text or variables to the terminal.
* **Why it matters:** It is used to display system variables (like `$PATH`) and is essential for creating automated security scripts.

  ![image alt](https://github.com/petersmuditha/Linux-for-cybersecutry/blob/0d8ed979dd37fe43dcf48b0d73b9e676b0888044/Cattura3.PNG)

### 6. `pwd` (Print Working Directory)
This command shows the full path of the directory you are currently working in.
* **Why it matters:** It provides essential context. Before running a command to delete or modify files, you must be certain of your exact location in the system.

  ![image alt](https://github.com/petersmuditha/Linux-for-cybersecutry/blob/0d8ed979dd37fe43dcf48b0d73b9e676b0888044/Cattura4.PNG)

## 🏁 Conclusion & Next Steps

This initial documentation covers the fundamental tools required to interact with a Linux system effectively. From basic navigation with `cd` and `ls` to advanced searching with `grep` and `find`, these commands form the foundation of any **Security Operations Center (SOC)** analyst or **Penetration Tester's** daily workflow.

## 💡 My Philosophy on Technical Writing

> *"I write for clarity and structure. I'm interested in how writing can influence behavior, simplify the complex, and shift how people understand security."*  
> — inspired by [ananichoumchoum](https://github.com/ananichoumchoum)

In cybersecurity, clear documentation saves time during incidents and ensures that knowledge isn't lost. Every project here is an exercise in making technical concepts accessible and actionable, just like the excellent walkthroughs on TryHackMe.

## 📬 Connect with Me

I'm actively looking for opportunities as a **Cybersecurity Technical Writer** or **Junior SOC Analyst**. If you have feedback on my work, want to collaborate, or know of an opportunity, I'd love to hear from you.

- Remote.com Link: [https://remote.com/jobs/account/profile]
- Email: petersmuditha@gmail.com

---

*Last updated:  23/03/2026*
*Documented by [Muditha Anuruddha Peters] during the TryHackMe Pre-Security Path.*
