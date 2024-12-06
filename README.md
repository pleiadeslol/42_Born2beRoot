# Born2beRoot - System Administration and Virtualization

**Born2beRoot** is a foundational project in system administration. It introduces students to virtualization and server configuration under strict rules, providing hands-on experience with essential system administration tools and concepts.

## 🚀 Project Overview

The project requires setting up a virtual machine using VirtualBox or UTM, configuring an operating system (Debian or Rocky Linux), and implementing various system administration tasks. The end goal is to create a secure and properly configured server environment.

## 🛠️ Key Features

### System Configuration
- **Virtual Machine Setup:**
  - Use VirtualBox (or UTM if VirtualBox is unavailable).
  - Operate without a graphical interface.
- **Operating System:**
  - Install the latest stable version of Debian (recommended) or Rocky Linux.
  - Configure AppArmor (Debian) or SELinux (Rocky) to run at startup.
- **Partitioning:**
  - Create at least two encrypted partitions using LVM.

### Security Measures
- **SSH Configuration:**
  - Run SSH on port 4242.
  - Disable root login via SSH.
- **Firewall:**
  - Configure UFW (Debian) or firewalld (Rocky) to only allow port 4242.
- **Password Policy:**
  - Enforce strong password rules (length, complexity, expiration, etc.).
- **Sudo Configuration:**
  - Restrict sudo usage with custom rules, logs, and error messages.

### Monitoring Script
Develop a Bash script, `monitoring.sh`, to display system statistics every 10 minutes, including:
  - OS architecture and kernel version.
  - CPU and memory usage.
  - Active connections and logged-in users.
  - Disk usage and LVM status.
  - IP and MAC address.
  - Commands executed with sudo.

### Submission Requirements
- Submit a single `signature.txt` file containing the SHA1 signature of your VM's virtual disk.
- Ensure the signature matches your VM during evaluation.

## 📜 Notes
- This project is shared for educational purposes as part of the 42 curriculum.
- During defense, expect questions about system configuration, SSH, and your monitoring script's functionality.

---

Happy configuring! 🚀
