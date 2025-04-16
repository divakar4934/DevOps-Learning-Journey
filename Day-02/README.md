# 📅 Day 02 - April 16, 2025

## 📘 What I Learned

Today I explored the basics of **Linux** and essential **Linux commands**  that is useful for anyone entering the DevOps world. Here's a breakdown of what I covered:

---

### 🐧 Linux Basics

#### 🔹 What is Linux?
Linux is a powerful open-source operating system used widely in servers, cloud infrastructure, and DevOps environments.

#### 🚀 Why is Linux Widely Used in DevOps?

Linux has become the **backbone of DevOps** and modern infrastructure for several key reasons:

✅ **Open Source & Free**  
- No licensing cost.  
- Highly customizable to fit different infrastructure needs.

✅ **Command-Line Power**  
- Most DevOps tools are CLI-based and Linux terminals are designed for power users.  
- Shell scripting (bash) makes automation easy.

✅ **Server Dominance**  
- A majority of cloud servers and enterprise environments run Linux-based distributions like Ubuntu, CentOS, RHEL, or Debian.

✅ **Tool Compatibility**  
- DevOps tools like Docker, Kubernetes, Jenkins, Ansible, Terraform, and more are **built for or run best on Linux**.

✅ **Stability & Security**  
- Linux is known for being **stable, lightweight, and secure**, making it ideal for production environments.

✅ **Automation Friendly**  
- Cron jobs, shell scripts, package managers (`apt`, `yum`) — all help automate tasks easily.

✅ **Cloud-Ready**  
- AWS, Azure, GCP — most cloud providers default to Linux-based instances.

> 💡 **Pro Tip:** If you're serious about DevOps, learning Linux is non-negotiable.

---

#### 🔹 File System Structure
- `/` – root directory  
- `/home/` – user directories  
- `/etc/` – config files  
- `/var/` – logs and variable data

---

### 📂 Navigation & File Management Commands

| Command | Description                         |
|---------|-------------------------------------|
| `pwd`   | Print current directory             |
| `ls`    | List files and directories          |
| `cd`    | Change directory                    |
| `mkdir` | Create new directory                |
| `touch` | Create empty file                   |
| `rm`    | Delete file                         |
| `cp`    | Copy files or directories           |
| `mv`    | Move or rename files/directories    |
| `clear` | Clear terminal screen               |
| `tree`  | Display directory structure (if installed) |

> 💡 Use `man <command>` to learn more about any command. Example: `man ls`

---

### 📁 File Viewing & Content Commands

| Command        | Description                             |
|----------------|-----------------------------------------|
| `cat`          | View content of file                    |
| `echo`         | Print text to terminal                  |
| `head` / `tail`| View start/end of file                  |
| `less` / `more`| Scrollable file viewing                 |
| `wc`           | Count lines, words, characters          |
| `grep`         | Search for patterns in files            |
| `nano`         | Command-line text editor (easy to use)  |
| `vim` / `vi`   | Advanced command-line text editor       |
| `emacs`        | Highly customizable text editor         |
| `sed`          | Stream editor for filtering and transforming text |
| `awk`          | Pattern scanning and processing language |
| `cut`          | Remove sections from each line of input |
| `sort`         | Sort lines of text                      |
| `uniq`         | Report or filter duplicate lines        |

---

### 🔄 Process Management

Understanding and managing running processes is a key skill in Linux system administration.

| Command      | Description                                      |
|--------------|--------------------------------------------------|
| `ps`         | View current running processes                   |
| `top`        | Real-time display of system processes            |
| `htop`       | Interactive process viewer (needs to be installed) |
| `kill`       | Terminate a process by PID                       |
| `killall`    | Terminate all processes by name                  |
| `nice`       | Start a process with a specific priority         |
| `renice`     | Change the priority of a running process         |
| `jobs`       | Show background jobs in current shell            |
| `fg`         | Bring a background job to foreground             |
| `bg`         | Resume a job in the background                   |

> 💡 Use `ps aux | grep <process>` to find a specific process.

---

### 💾 Disk Management

Managing disk space and understanding file system usage is crucial in maintaining a healthy server environment.

| Command        | Description                                      |
|----------------|--------------------------------------------------|
| `df -h`        | Show disk space usage in human-readable format   |
| `du -sh <dir>` | Show space used by a directory                   |
| `mount`        | List mounted file systems                        |
| `umount`       | Unmount a mounted file system                    |
| `lsblk`        | Display info about block devices (disks)         |
| `fdisk -l`     | Show disk partitions (requires sudo)             |
| `blkid`        | Display UUIDs of partitions                      |
| `parted`       | Manage disk partitions (interactive)             |
| `df -i`        | Show inode usage                                 |
| `mkfs`         | Create a new filesystem on a partition or disk   |
| `fsck`         | Check and repair filesystem integrity            |


> 💡 Regularly checking disk usage helps prevent server crashes due to full partitions.

---

### 🌐 Networking

Networking is an essential part of DevOps, especially when dealing with distributed systems, cloud environments, and microservices.

| Command               | Description                                             |
|-----------------------|---------------------------------------------------------|
| `ip a`                | Show network interfaces and their IP addresses          |
| `ifconfig`            | Deprecated, used to configure network interfaces        |
| `ping <host>`         | Check connectivity to another host (e.g., `ping google.com`) |
| `netstat -tuln`       | Show open ports and listening services                  |
| `ss`                  | Socket statistics (modern alternative to `netstat`)     |
| `traceroute <host>`   | Trace the path to a network host                        |
| `nslookup <domain>`   | Query DNS for a domain                                 |
| `dig <domain>`        | DNS lookup and query tool                              |
| `curl <url>`          | Transfer data from or to a server (useful for APIs)    |
| `wget <url>`          | Download files from the web                             |
| `scp <source> <user>@<host>:<destination>` | Securely copy files between local and remote systems |
| `ssh <user>@<host>`   | Securely connect to a remote server via SSH            |
| `route`               | Show or manipulate the IP routing table                |

> 💡 **Pro Tip:** Use `ping -c 4 <host>` to limit the number of ping attempts to 4 packets.

---


### 🔐 File Permissions

| Symbol | Meaning       |
|--------|---------------|
| `r`    | Read          |
| `w`    | Write         |
| `x`    | Execute       |

#### Commands:
- `ls -l` → Show detailed list with permissions  
- `chmod +x script.sh` → Make file executable  
- `chmod 755 filename` → Set read/write/execute permissions

---
