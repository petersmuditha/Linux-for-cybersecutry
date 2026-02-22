# 🐧 Linux Fundamentals

**A practical guide and portfolio of log analysis projects for aspiring Cybersecurity Technical Writer**

👋 Hi, I'm Muditha an aspiring  **Cybersecurity Technical Writer**.  
This repository is my learning journal and portfolio, where I document my journey in mastering log analysis, from basic Linux commands to advanced SIEM investigations, based on the **TryHackMe SOC Level 1 path**.

I believe that **good documentation is as important as good detection**. Here you'll find not just commands, but structured methodologies, real-world use cases (with fake data), and reusable templates that I've built to help others (and myself) respond faster and smarter.

---

## 🛠️ Skills & Tools (TryHackMe-aligned)

🔹 **Core Linux Navigation: Essential commands for navigating the filesystem (cd, ls, pwd, cat).** 
🔹 **File Management and Search: Creating, moving, copying, and deleting files and directories (touch, mkdir, cp, mv, rm). Using powerful search tools such as find and grep.** 
🔹 **Understanding the Linux Filesystem: Understanding standard Linux directories and their purposes (e.g., /etc, /var, /tmp).**   
🔹 **Permission Management: Understanding and managing file and folder permissions (read, write, execute), and an introduction to user and group management.**   
🔹 **Shell Operations and Automation: Using shell operators (&, &&, >, >>) to run commands in the background and chain them together. Introduction to basic scripting concepts.**  
🔹 **Remote Access: Using SSH (Secure Shell) to connect to and administer Linux machines remotely.** 
🔹 **Command-Line Proficiency: Ability to use the built-in manual (man) and command options (flags and switches) to discover and use advanced features.**

---

## 🧭 About This Repository

This repository is structured to reflect the core modules of the **Linux fundamentals part 1 & 2**, with practical projects for each area.

 The goal is to demonstrate a solid working understanding of fundamental Linux concepts, which are the foundation for any role in cybersecurity and system administration. The projects contained here demonstrate the practical application of these concepts, from basic filesystem navigation to managing permissions and remote connections

---

## 🚨 Projects & Use Cases (TryHackMe-based)

- Linux Filesystem Exploration	Linux Fundamentals Part 1	cd, ls, pwd, cat, find	Practical application of commands to navigate the directory structure of a Linux system and locate specific files.

- Introduction to Shell Operators]	Linux Fundamentals Part 1	&, &&, >, >>	Hands-on examples of running commands in the background and redirecting command output to automate simple tasks.
  
- User and Permission Management	Linux Fundamentals Part 2	ls -lh, chmod, file, User/Group concepts	Practical demonstration of how to view and modify access permissions for files and directories — a key security concept.

- Remote Administration via SSH	Linux Fundamentals Part 2	ssh, whoami, basic network commands	Walkthrough on establishing a secure SSH connection to a remote machine and executing administration commands, simulating server management.

- Pattern Searching & Log Analysis 101	Linux Fundamentals Part 1	grep, find, output redirection	Using grep and find to search for specific strings within files — a foundational skill for starting to analyze system logs.

> 🔒 *All data used in these projects is 100% synthetic and generated in isolated lab environments (TryHackMe rooms, custom VMs). No real customer or company data is ever used.*

---

## 📚 What I'm Learning & Demonstrating

Through this repository, I intend to demonstrate:

Solid Linux Foundation: Not just theoretical knowledge, but practical ability to interact with a Linux system using the command line, navigate the filesystem, manage files, and understand basic security mechanisms.

Understanding Key Security Concepts: Mastery of elements such as user and permission management, which are essential for understanding how to isolate and protect processes and data on a system.

Remote Administration Approach: Demonstration of practical skills in using SSH for system management, a daily activity for those working with servers and IT infrastructure.

Problem-Solving with the Shell: Ability to use commands such as grep and find to solve real-world problems, such as finding a file or extracting specific information from a log, laying the foundation for future analysis.

Clear and Structured Documentation: The very organization of this repository serves to demonstrate my ability to document my work clearly and accessible, a crucial skill for any technical team.

---

## ⚠️ Disclaimer

All data, logs, and scenarios in this repository are **fictional and generated in controlled lab environments** (TryHackMe rooms or custom VMs). They do not contain any sensitive information from real organizations or individuals. The purpose is purely educational and for portfolio demonstration.

---

Special thanks to **TryHackMe** for providing an incredible hands-on learning platform that makes cybersecurity accessible to everyone.

---

## 🛡️ Beyond the Surface: Linux vs. Windows
Linux is often perceived as more intimidating or complex than familiar operating systems like *Windows*. However, both platforms offer unique strengths: while Windows focuses on user-friendliness, Linux stands out for being **extremely lightweight**, highly customizable, and robust.

## 🌍 An Invisible but Constant Presence
Without realizing it, you interact with Linux almost every second of your day. It’s not just a tool for "hackers"; it is the engine driving the modern world:

* **🌐 The Web:** The vast majority of websites you visit daily run on Linux-based servers.
* **🚗 Automotive:** From infotainment systems to vehicle control panels, the software core is often powered by Linux.
* **🛒 Retail & Commerce:** Point of Sale (PoS) systems and automated checkouts rely on its stability and security.
* **🏗️ Critical Infrastructure:** Industrial sensors and traffic light controllers are managed by specialized Linux distributions.

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
