# 🔍 Task 1 - Scan Your Local Network for Open Ports

## 📌 Project Overview
This project demonstrates how to **scan a local network for open ports** using **Nmap on Ubuntu Linux**.

The main objective is to identify:
- Active devices in the local subnet
- Open TCP ports
- Running services
- Potential security exposure points

This task helps in understanding **network reconnaissance and attack surface analysis**, which is an important concept in cybersecurity.

---

## 🎯 Objective
To discover open ports on devices in the local network and analyze exposed services for security awareness.

---

## 🛠️ Tools & Technologies
- Ubuntu Linux
- Nmap
- ip addr
- ifconfig
- Terminal

---

## 🌐 Network Configuration
The local machine network details:

- **IP Address:** `10.0.2.15`
- **Subnet Mask:** `255.255.255.0`
- **Broadcast:** `10.0.2.255`

Subnet scanned:

```bash
10.0.2.0/24
```

---

## ⚙️ Commands Used

### Check IP Address
```bash
sudo ip addr show
```

### View Interface Details
```bash
sudo ifconfig
```

### Install Nmap
```bash
sudo apt-get install nmap
```

### Scan Entire Local Network
```bash
nmap 10.0.2.0/24
```

### Scan Specific Host
```bash
nmap 192.168.0.2
```

### Scan Specific Port
```bash
nmap -p 3000 172.16.60.182
```

---

## 📊 Open Ports Identified
The scan discovered several important services:

| Port | Service |
|---|---|
| 21 | FTP |
| 22 | SSH |
| 23 | Telnet |
| 53 | DNS |
| 80 | HTTP |
| 135 | MSRPC |
| 139 | NetBIOS |
| 389 | LDAP |
| 443 | HTTPS |
| 445 | Microsoft-DS |
| 3306 | MySQL |
| 3389 | RDP |
| 5432 | PostgreSQL |
| 8080 | HTTP Proxy |

---

## 🔐 Security Analysis
The following risks were observed:

- FTP may allow insecure file transfer
- SSH can be brute-force targeted
- Telnet is insecure and outdated
- MySQL/PostgreSQL exposure risks database leaks
- RDP can allow unauthorized remote access
- LDAP ports may expose directory services

---

## 📷 Output Screenshots
The repository includes:
- Terminal screenshots
- Nmap subnet scans
- Host-specific port scans
- PDF task report

---

## 📚 Learning Outcomes
Through this task, I learned:

- How subnet scanning works
- Service enumeration using Nmap
- Identifying live hosts
- Detecting exposed services
- Understanding network vulnerabilities
- Basics of ethical reconnaissance

---

## 📂 Repository Structure
```bash
├── README.md
└── elevate_labs_d1_task1.pdf
```

---

## 👨‍💻 Author
**Devansh Savla**  
Cybersecurity / Networking Task - Elevate Labs
