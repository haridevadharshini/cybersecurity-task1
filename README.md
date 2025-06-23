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
