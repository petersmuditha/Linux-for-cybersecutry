# 🐧 Linux Fundamentals

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

### 1. The `whoami` Command
The `whoami` command answers a vital question: *"Which user am I currently logged in as?"*

* **Usage:** Simply type `whoami` in the terminal.
* **Security Relevance:** In a penetration test or a security audit, the first thing you need to know is your privilege level. Knowing if you are a low-privileged user or the **root** (administrator) determines your next moves.

![image alt](https://github.com/petersmuditha/Linux-for-cybersecutry/blob/0d8ed979dd37fe43dcf48b0d73b9e676b0888044/Cattura2.jpg)

### 2. The `echo` Command
The `echo` command is used to print text or variables directly to the terminal output.

* **Example:** Running `echo "Linux is awesome"` will display that exact string on your screen.
* **Security Relevance:** Beyond simple printing, `echo` is essential in **automation scripts**. It is used to create configuration files on the fly or to verify system environment variables during a security hardening process.

![image alt](https://github.com/petersmuditha/Linux-for-cybersecutry/blob/0d8ed979dd37fe43dcf48b0d73b9e676b0888044/Cattura3.PNG)

## 📂 File System Navigation

To move around the Linux file system and interact with files, we use a set of core navigation commands. Mastering these is the first step toward effective system administration and security auditing.

### 1. The `pwd` Command (Print Working Directory)
Before moving anywhere, you need to know where you are. `pwd` shows the full path of your current directory.
* **Usage:** `pwd`
* **Why it matters:** In cybersecurity, you must always be aware of your location to avoid running scripts or deleting files in the wrong directory.

![image alt](https://github.com/petersmuditha/Linux-for-cybersecutry/blob/0d8ed979dd37fe43dcf48b0d73b9e676b0888044/Cattura4.PNG)

### 2. The `ls` Command (List)
The `ls` command reveals the contents of a directory (files and folders).
* **Usage:** `ls` (or `ls -la` to see hidden files and detailed permissions).
* **Why it matters:** Attackers often hide malicious files by starting the filename with a dot (e.g., `.hidden_malware`). Using `ls -la` allows a security analyst to spot these hidden threats.

![image alt](https://github.com/petersmuditha/Linux-for-cybersecutry/blob/0d8ed979dd37fe43dcf48b0d73b9e676b0888044/Cattura5.PNG)

### 3. The `cd` Command (Change Directory)
The `cd` command allows you to move between folders.
* **Usage:** `cd [directory_name]` (e.g., `cd /var/log`).
* **Why it matters:** Navigating to log directories is a daily task for a security writer documenting incident response steps.

![image alt](https://github.com/petersmuditha/Linux-for-cybersecutry/blob/0d8ed979dd37fe43dcf48b0d73b9e676b0888044/Cattura6.PNG)

### 4. The `cat` Command (Concatenate)
The `cat` command is the quickest way to read the contents of a file without opening an editor.
* **Usage:** `cat [filename]` (e.g., `cat flag.txt`).
* **Why it matters:** On TryHackMe, `cat` is your best friend for reading "flags." In the real world, it’s used to quickly inspect configuration files or system logs for suspicious activity.

![image alt](https://github.com/petersmuditha/Linux-for-cybersecutry/blob/0d8ed979dd37fe43dcf48b0d73b9e676b0888044/Cattura7.PNG)

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

*Last updated:  22/02/2026*
*Documented by [Muditha Anuruddha Peters] during the TryHackMe Pre-Security Path.*
