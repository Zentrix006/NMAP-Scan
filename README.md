# NMAP-Scan

# 🔍 Local Network Port Scanning with Nmap

## 📋 Objective
This task focused on learning **network reconnaissance** by scanning the local network for **open ports** and identifying potential security risks. Using **Nmap**, I performed a TCP SYN scan (`-sS`) across my local network (`192.168.31.0/24`).

---

## 🛠️ Tools Used
- **Nmap 7.95** - For scanning the network and discovering open ports.


---

## 🌐 Local Network Scan
The scan identified **3 active devices** with open ports and services.  
To maintain privacy, I’ve **redacted sensitive information** such as MAC addresses.  
Here’s a summary of what was found:

- **Router/Gateway** (`192.168.31.1`)  
  Open Ports: 53 (DNS), 80 (HTTP), 443 (HTTPS), 7443, 8080, 8443  

- **Device 2** (`192.168.31.59`)  
  Open Ports: 903, 5357  

- **My Machine** (`192.168.31.239`)  
  No open ports detected.

---

## 🔐 Key Concepts Learned
- **Port Scanning**: Identifying which ports on a device are open to understand potential exposure.
- **TCP SYN Scan (`-sS`)**: A stealthy scan that sends SYN packets to see if ports are open without completing the TCP handshake.
- **Local IP Range**: Discovered using `ifconfig` or `ip addr`, which in my case was `192.168.31.0/24`.
- **Network Reconnaissance**: Understanding which devices and services are accessible on the local network.
- **Security Risks**: Open ports can be entry points for attacks. It’s crucial to secure services or restrict access.
---
## 🖥 Nmap Command Used
```bash
sudo nmap -sS 192.168.31.0/24 -oN scan_results.txt
```
---

## 📤 Files in This Repository
- `scan_results.txt`: Contains the **redacted Nmap scan output** of my local network.
- `README.md`: This document summarizing the task.


## 📌 Submission Notes
I’ve redacted sensitive information (e.g., MAC addresses) for security before uploading to this repository.

---

🔗 **Task Completed!**
