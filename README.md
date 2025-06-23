# 🔐 Cyber Security Internship - Task 1: Network Reconnaissance

## 🎯 Objective

Perform a TCP SYN scan on a local network using Nmap, capture traffic with Wireshark, identify reachable hosts, and understand common services and their potential risks.

---

## 🛠 Tools Used

- 🐧 Kali Linux
- 🔍 Nmap
- 📡 Wireshark

---

## 🧪 Steps Performed

1. Identified my network IP range using `ip a`
2. Ran a TCP SYN scan using:
   ```bash
   sudo nmap -sS 192.168.1.0/24 -oN network_scan.txt

# Network Security Scan Analysis

## 🔍 Scan Overview
| Parameter        | Value                     |
|------------------|---------------------------|
| Scan Type        | TCP SYN Stealth Scan (`-sS`) |
| Target Network   | 192.168.37.0/24           |
| Tool Version     | Nmap 7.95 (Kali Linux)    |
| Scan Duration    | 8.55 seconds              |
| Total Hosts Scanned | 256                     |

## 📊 Findings Table
| Host IP        | Status   | Open Ports | Filtered Ports | Closed Ports | Notable Services |
|----------------|----------|------------|----------------|--------------|------------------|
| 192.168.37.1   | Active   | 0          | 1000           | 0            | None             |
| 192.168.37.2   | Active   | 0          | 1              | 999          | DNS (53/tcp)     |
| 192.168.37.254 | Active   | 0          | 1000           | 0            | None             |
| 192.168.37.128 | Active   | 0          | 0              | 1000         | None             |

## 🛡️ Security Assessment
```text
✅ All hosts properly firewalled  
✅ Zero exposed services  
✅ Only essential filtered services (DNS)  
✅ No unexpected devices detected  
